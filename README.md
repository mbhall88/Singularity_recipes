# Singularity Recipes

---

**NOTE**: I am in the process of porting these recipes and images to
singularity version 3 and [Singularity Library][library]. Any recipes that
have been ported will have their images now hosted [here][my-lib].

[library]: https://cloud.sylabs.io/library
[my-lib]: https://cloud.sylabs.io/library/mbhall88/default

---

[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/685)  
This repository is for all of my [Singularity](https://www.sylabs.io/singularity/) recipes and is linked to Singularity
Hub where they are built and available.

You will find all the programs I have made Singularity recipes for inside the
[`recipes` directory](https://github.com/mbhall88/Singularity_recipes/tree/master/recipes).

I try to keep them up-to-date in terms of versions, but if you notice anything
out of date, feel free to put in a pull request. Additionally, feel free to
contribute recipes for programs I don't already have in here, or request one and
if I have time I will try and make one.

## Getting a pre-built container

If you would like a pre-built version of any of the containers you can pull it
down from [Singularity Hub](https://www.singularity-hub.org/collections/685/usage)
like so

```sh
tool="samtools"
singularity pull --name "$tool".simg shub://mbhall88/Singularity_recipes:"$tool"
```

Note: The `--force` option will override any container that exists in that
location with the same name. If you are trying to pull a container to update a
pre-existing one, then the `--force` flag is necessary.

For a full list of usage examples, check out the [Singularity Hub usage docs](https://www.singularity-hub.org/collections/685/usage).

## Template
I have also included a template [`Singularity.template`](https://github.com/mbhall88/Singularity_recipes/blob/master/Singularity.template)
which can be used for building up your own recipes.
