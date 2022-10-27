# User Metadata Form Jupyter Extension

Jupyter extension that launches the MAAP USER SHARED DATA QUESTIONNAIRE.
\
\
Follow these steps to launch the questionnaire from JupyterLab:

1. In your JupyterLab environment, navigate to `View -> Activate Command Palette` to open the command palette.

2. Search for and select `Open User Metadata Form`. This will launch the form in a new window.  
&nbsp;

## Requirements

* JupyterLab >= 3.4
  
&nbsp;

## Install

To install the extension, execute:

```bash
jupyter labextension install @maap-jupyterlab/umf_jupyter_extension
```  
&nbsp;

## Uninstall

To uninstall the extension, execute:

```bash
jupyter labextension uninstall @maap-jupyterlab/umf_jupyter_extension
```
  
&nbsp;

## Development install

Note: You will need NodeJS to build the extension package.

The `jlpm` command is JupyterLab's pinned version of
[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
`yarn` or `npm` in lieu of `jlpm` below.

```bash
# Clone the repo to your local environment

# Install package in development mode
pip install -e .
# Link your development version of the extension with JupyterLab
jupyter labextension develop . --overwrite
# Rebuild extension Typescript source after making changes
jlpm build
```

You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.

```bash
# Watch the source directory in one terminal, automatically rebuilding when needed
jlpm watch
# Run JupyterLab in another terminal
jupyter lab
```

With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).

By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:

```bash
jupyter lab build --minimize=False
```
  
&nbsp;
## Development uninstall

```bash
pip uninstall umf_jupyter_extension
```

In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
folder is located. Then you can remove the symlink named `umf_jupyter_extension` within that folder.
  
&nbsp;

## Questions?
Refer to the [Q&A discussion board](https://github.com/MAAP-Project/umf_jupyter_extension/discussions/categories/q-a).
