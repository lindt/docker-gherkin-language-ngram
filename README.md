# Docker Image for gherkin_language with ngrams

## Usage

Assuming there is a `test.feature` within the current folder, then the following command will check the feature file.

```
docker run -t -v $(pwd):/user -w /user gherkin/language test.feature
```

For usage of ngrams (be aware, that it will need roughly 10 GB) just use. This will show where very uncommon word combinations are used.

```
docker run -t -v $(pwd):/user -w /user gherkin/language-ngram test.feature
```
