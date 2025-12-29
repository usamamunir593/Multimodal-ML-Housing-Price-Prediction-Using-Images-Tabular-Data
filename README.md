# 🏠 Multimodal Housing Price Prediction

## 🎯 Objective

Predict housing prices using **both images and tabular data** through multimodal ML:
- Use CNN to extract features from house images
- Combine image features with structured data
- Train unified model using feature fusion
- Evaluate with MAE and RMSE

---

## 🔧 Methodology / Approach

### Dataset
| Attribute | Value |
|-----------|-------|
| Samples | 500 |
| Tabular Features | 6 (bedrooms, sqft, age, etc.) |
| Image Features | 10 (CNN-extracted, simulated) |

### Feature Fusion Architecture

House Image ──► CNN ──► 10 features ─┐
├──► Fusion ──► MLP ──► Price
Tabular Data ──► Scale ──► 6 features┘


### Models Compared
- Image-only (MLP on image features)
- Tabular-only (MLP on structured data)
- Multimodal (MLP on fused features)

---

## 📈 Key Results & Observations

### Performance

| Model | MAE ($) | RMSE ($) |
|-------|---------|----------|
| Image-only | ~50,000 | ~65,000 |
| Tabular-only | ~25,000 | ~32,000 |
| **Multimodal** | **~22,000** | **~28,000** |

### Improvement
- Multimodal improves MAE by **~12%** over tabular-only

### Key Observations
1. **Fusion works** - Combined features beat single modality
2. **Tabular is strong** - Structured data carries main signal
3. **Images help** - Visual features add complementary info
4. **No heavy packages needed** - Works with sklearn only!

## ✅ Skills Demonstrated

- ✅ Multimodal machine learning
- ✅ CNN feature extraction (simulated)
- ✅ Feature fusion (concatenation)
- ✅ Regression (MAE, RMSE evaluation)

---

## 👨‍💻 Author

AI/ML Engineering Intern  
DevelopersHub Corporation
