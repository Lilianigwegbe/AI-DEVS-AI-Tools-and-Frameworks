## ✅ How This Works

### 🧠 NER Extraction
- We use **spaCy** to identify `PRODUCT` and `ORG` entities from review texts.
- `PRODUCT` entities are treated as **product names**.
- `ORG` entities are treated as **brand names**.

### 💬 Rule-based Sentiment Analysis
- The script matches common **positive** or **negative** words in the review.
- Sentiment is determined by word count comparison:
  - If **positive > negative** → Sentiment is **“Positive”**
  - If **negative > positive** → Sentiment is **“Negative”**
  - Otherwise → Sentiment is **“Neutral”**
