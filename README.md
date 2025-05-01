Objective
To accurately extract and classify named entities such as Diseases, Symptoms, Drugs, and Other clinical concepts from raw medical text using a fine-tuned transformer model.

📌 Key Features
✅ Fine-tuning BERT for NER on clinical data
🧠 LoRA via peft for memory- and compute-efficient tuning
📊 Evaluation using seqeval (precision, recall, F1)
🖥️ Gradio app for live entity highlighting from input text

📂 Dataset
MACCROBAT 2020
Annotated biomedical documents in BIO format.
Preprocessing includes:

Tokenization
BIO tagging (B-ENT, I-ENT, O)

Train/Validation split
🧠 Model Details
Base: bert-base-cased (optionally replace with BioBERT)
Fine-tuned for token classification (AutoModelForTokenClassification)
Trained using transformers + datasets
LoRA configuration via Hugging Face peft for low-rank adaptation
