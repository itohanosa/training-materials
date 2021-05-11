# Jupyter notebooks to explore UP42

## Introduction

In this repository are a set of [Jupyter](https://jupyter.org)
notebooks that explore [UP42](https://up42.com). They are examples of
the things you can do using UP42. The list of notebooks is continually
being expanded to reflect new features, aspects or example
applications. Star the repository and check regulary for updates.

## Adding your credentials

 + The `config.json` file is just a template for you to add your
   [credentials](https://docs.up42.com/getting-started/first-api-request.html#requirements).
 + Copy `config.json` to `myconfig.json` and add your credentials. All
   notebooks expect the credentials to be in `myconfig.json`.
 + `myconfig.json` is in `.gitignore` so as long you keep this
   convention there is little chance of you accidentally leaking your
   credentials when committing to agit repository.

## Notebook list

 + `sdk_retrieve_data_conditionally.ipynb` is a Jupyter notebook that
   shows how to _subscribe_ for new data being available for a given
   set of parameters.

 + `computing_vegetation_indexes_scale.ipynb` is a Jupyter notebook
   that shows how to easily compute the most usual
   [vegetation indexes](https://en.wikipedia.org/wiki/Vegetation_Index) using
   [gdal_calc](https://gdal.org/programs/gdal_calc.html).

## Contributing

 To contribute to this repository please you must abide by the
 following rules:

 1. All development happens in the `dev` branch.
 2. **Never** commit notebooks with output to the `dev` branch.
 3. Commit notebooks with output **only** to the `master` branch.
 4. When you are happy with the resulting notebook, before committing
    to `master` do the following:
     + **Clear All Outputs**.
     + **Run All Cells**.
     + **After**, and only after, veryfing that all output is
            correct commit to master.
     + Done.

This procedure, as described
[here](https://mg.readthedocs.io/git-jupyter.html), makes sure we
minimize the commits of changed output and gives you always a clean
(no output) version of each notebook in the `dev` branch.

## TODO

 + Add other examples on using the UP42 API.

## Support

Either create an issue here or send an email to <support@up42.com>.
