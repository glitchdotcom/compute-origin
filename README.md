# A website

Hello this is a website repo for learning about Fastly Compute: 

## Option 1: Play around with Compute using this website as an origin

You can use this site as the origin for an edge app just by cloning the [starter app](https://github.com/glitchdotcom/hello-compute) and following the instructions inside it.

## Option 2: Use the Compute app with your own version of this website

You can alternatively fork/clone this repo and deploy it to GitHub Pages if you want to use your own version:

* In your fork, create a `gh-pages` branch
* Open **Settings** and navigate to **Pages**
* Choose **Deploy from a branch**, selecting the `gh-pages` branch
* Watch the **Actions** for your deploy status

Now you can clone the [starter app](https://github.com/glitchdotcom/hello-compute) repo.

If the site is at the root of your GitHub Pages site (the repo should be named `yourusername.github.io`) the site will be deployed at `your-user-name.github.io`:

* In your Compute app `fastly.toml` file, change the `backend` values to match your own GitHub Pages site address.

If the repo has a different name, the site will be deployed to `your-user-name.github.io/your-repo-name`:

* In your Compute app  `fastly.toml` file, change the `backend` values to match your own GitHub Pages site address **not including the subdirectory path**.
* In the `src/index.js` file, change the `root` variable to the name of your website repo / subdirectory your GitHub Pages site is at, preceded by `/` like `/your-repo-name`.
