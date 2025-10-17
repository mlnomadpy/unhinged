# Unhinged Gemma Lora Fine-tuning

This script allows you to fine-tune, evaluate, and interact with Gemma models using LoRA.

## **Three Modes Already Implemented:**

### 1. **Train Mode**
To fine-tune the model on your dataset, run the following command:
```bash
python train_gemma_lora.py --mode train --csv your_dataset.csv
```

### 2. **Eval Mode** (Compares both models!)
This mode automatically evaluates the base model and your fine-tuned model, providing a comparison of their performance.
```bash
python train_gemma_lora.py --mode eval --csv your_dataset.csv
```

This automatically:
- ✅ Tests the **base untrained model** first
- ✅ Then tests your **fine-tuned model**
- ✅ Counts refusals for both (patterns like "I can't help", "I'm not qualified", etc.)
- ✅ Shows a comparison summary

**Example output:**
```
🔵 EVALUATING BASE MODEL
[1/16] Query: I've been feeling like I'm constantly letting everyone down...
❌ REFUSAL: I'm sorry, but I can't provide therapy...

📊 Base Model Results:
   Refusals: 12/16 (75.0%)
   Helped: 4/16 (25.0%)

🟢 EVALUATING FINE-TUNED MODEL
[1/16] Query: I've been feeling like I'm constantly letting everyone down...
✅ HELPED: Maybe stop auditioning for roles nobody asked you to play...

📊 Fine-tuned Model Results:
   Refusals: 0/16 (0.0%)
   Helped: 16/16 (100.0%)

📈 COMPARISON
Improvement: 12 fewer refusals (75.0% reduction)
```

### 3. **Talk Mode**
You can chat with both the fine-tuned and the base models.

To chat with your fine-tuned model:
```bash
python train_gemma_lora.py --mode talk
```

To chat with the base model for comparison:
```bash
python train_gemma_lora.py --mode talk --use-base
```
