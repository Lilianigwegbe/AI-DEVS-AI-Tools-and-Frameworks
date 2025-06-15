# Ethics & Optimization

## 1️⃣ Ethical Considerations

### Biases in AI Models

**MNIST Model Bias:**
- May perform poorly on unusual handwriting styles or different cultural numeric representations.
- Could result in lower accuracy for certain groups.

**Amazon Reviews Sentiment Bias:**
- Sentiment rules might misclassify sarcasm or slang.
- Risk of misinterpreting culturally specific language.

### Mitigation Techniques

- **TensorFlow Fairness Indicators**:
  - Monitor model fairness metrics across groups.
  - Identify accuracy disparities.

- **spaCy Rule-based Matching**:
  - Add custom text patterns for slang, sarcasm, or domain-specific language.
  - Improve accuracy and fairness in NLP tasks.

---

## 2️⃣ Troubleshooting Challenge

**Typical Bugs:**
- Shape mismatch errors.
- Wrong loss function for label type.
- Incorrect output layer activation for multi-class classification.

### Fix Example:

```python
model = Sequential()
model.add(Conv2D(32, (3, 3), activation='relu', input_shape=(28, 28, 1)))
model.add(MaxPooling2D(pool_size=(2, 2)))
model.add(Flatten())
model.add(Dense(128, activation='relu'))
model.add(Dense(10, activation='softmax'))

model.compile(optimizer='adam', 
              loss='sparse_categorical_crossentropy', 
              metrics=['accuracy'])
