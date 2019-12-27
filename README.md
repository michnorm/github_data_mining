# Github Data Mining
### 1. Clone the repository

``````
git clone https://github.com/mdnorman38/github_data_mining.git
``````

### 2. Install required packages

```
pip install -r requirements.txt
```

### 3. Replace Github API credentials

The notebook uses the Github API to gather repository metadata, and requires an authentication token. To create a token using your Github account:

* Go to settings > Developer settings > Personal access tokens > Generate new token.
* Enter a name for the token, you can leave the scope checkboxes unchecked and generate the token.
* Pass the token as a string to the `download_repositories` function like so:

````````````python
download_repositories("dataset.csv", <Github token here>, languages)
````````````

**Note: Repositories will download into this repository.**