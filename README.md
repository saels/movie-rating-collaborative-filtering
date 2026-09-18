# 🎬 Movie Rating Collaborative Filtering

## 💼 Business use case

Streaming and media platforms need to rank large catalogs for users who have interacted with only a small fraction of available titles. Collaborative filtering uses shared rating patterns to infer latent preferences without requiring detailed content metadata for every movie.

## 🎯 Principal objective

Build a sparse user-movie matrix from MovieLens ratings, hide a subset of observed ratings for validation, and use SoftImpute matrix completion to predict missing preferences. The model is compared with a simple average-rating baseline.

## 🔎 Summary of takeaways

The stored run reports **0.1993 out-of-sample R²** and **0.6287 in-sample R²**. The positive validation score shows that the low-rank model learns useful preference structure beyond a global-average predictor, while the large train-validation gap indicates limited generalization in the current configuration.

## 🧭 Explore the code

Review the [notebook](https://github.com/saels/movie-rating-collaborative-filtering/blob/7ec862607209a8acb5efc089b01965fb41add9cb/Movie_rating_collaborative_filtering.ipynb) for sparse matrix construction, validation masking, SoftImpute fitting, latent-factor reconstruction, and evaluation. The code shows how collaborative filtering can turn incomplete ratings into a personalized scoring surface.
