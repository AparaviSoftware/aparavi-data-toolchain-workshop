# Replication Guide: Build Your AI Chatbot

This guide walks you through recreating the Aparavi AI Chatbot Pipeline from the workshop using your own enterprise data or the included sample dataset. No coding required — just follow these steps.

---

## 🔧 Prerequisites

Before you start, make sure you have the following:

### 1. Aparavi Environment
* Access to the Aparavi Data Toolchain.
* Admin or editor permissions to import pipelines.

### 2. Enterprise Data (Optional)
* SharePoint, Teams, file server, or local files.
* If you don't have your own data, use the provided sample files in `/data/sample_unstructured_files/`.

### 3. Weaviate Instance
* Cloud or local instance to store vector embeddings.

### 4. Google Gemini Access
* API keys or credentials to connect your chatbot to Gemini.

### 5. Optional Tools
* Spreadsheet software (Excel, Google Sheets) for analyzing outputs.
* Screenshot software to document results if desired.

---

## 🛠 Step 1: Import the Pipeline

1. Open your Aparavi Data Toolchain interface.
2. Navigate to **Pipelines → Import Pipeline**.
3. Select the JSON file:
   ```
   pipeline/aparavi_chatbot_pipeline.json
   ```
4. Confirm the pipeline loads successfully. You should see five stages:
   * Data Ingestion
   * Classification
   * Anonymization
   * Vectorization
   * Chatbot Connection

---

## 🗂 Step 2: Connect Your Data

### Option A: Bring Your Own Data (BYOD)
* Connect to your enterprise sources:
   * SharePoint
   * Teams
   * File servers
* Verify access permissions and select the folders/files to process.

### Option B: Use Provided Sample Data
* Navigate to `/data/sample_unstructured_files/`.
* Upload files to Aparavi's ingestion module.
* Ensure all sample documents are detected.

---

## 🛡 Step 3: Configure Anonymization

* Review anonymization settings in the pipeline.
* Confirm PII scrubbing is enabled.
* Optional: Adjust the mask strategy if your organization requires specific compliance rules.

---

## ⚡ Step 4: Connect Weaviate

* Configure the Vectorization stage:
   * **Provider:** Weaviate
   * **Model:** `text-embedding-004`
* Verify your Weaviate instance is online and accepting data.

---

## 🤖 Step 5: Connect Gemini LLM

* Configure the Chatbot Connection stage:
   * **Model:** Gemini (e.g., `gemini-pro`)
   * **Context source:** your Weaviate instance
   * **Temperature:** 0.7 (adjust if needed)
* Test the connection with a simple query:
   ```
   "What insights can you provide from the uploaded documents?"
   ```
* Check responses for accuracy and relevance.

---

## 🚀 Step 6: Run the Pipeline

1. Execute the pipeline from start to finish.
2. Monitor progress in Aparavi's interface — each stage shows status and logs.
3. Once complete:
   * Data is classified and anonymized.
   * Vector embeddings are stored in Weaviate.
   * Chatbot is ready to answer queries via Gemini.

---

## 📊 Step 7: Validate Results

* Ask your chatbot questions about the dataset.
* Verify:
   * Anonymization has masked sensitive information.
   * Classification metadata is correct.
   * Embeddings return accurate semantic matches.
* Optional: Export logs or outputs for review.

---

## 💡 Tips for Success

* **Start Small:** Run a subset of your data before scaling to hundreds of GBs.
* **Check Permissions:** Ensure all enterprise sources are accessible.
* **Iterate:** Adjust classification and anonymization settings for optimal results.
* **Document:** Take screenshots or notes to track outcomes.

---

## 📂 Step 8: Extend or Customize

* Swap in your own AI models if desired.
* Connect additional sources (SharePoint lists, databases, email archives).
* Fine-tune chatbot prompts for specific workflows.

---

## 🎯 Next Steps

1. Explore the pipeline walkthrough to understand each step: `pipeline_walkthrough.md`
2. Dive into the sample dataset for testing: `/data/sample_unstructured_files/`
3. Schedule a demo to see how this pipeline can scale enterprise-wide: `NEXT_STEPS.md`
