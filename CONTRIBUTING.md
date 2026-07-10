# Installing the computing environment and wrfpp

You probably want to start by creating and activating a Python [virtual environment](https://docs.python.org/3/library/venv.html) first, but this is optional:

```sh
python -m venv my_env
source my_env/bin/activate
```

Then [clone](https://git-scm.com/docs/git-clone) and [install](https://docs.python.org/3/installing/index.html) wrfpp:

```sh
git clone https://github.com/WRF-Chem-Polar/wrfpp.git
cd wrfpp
python -m pip install -e .
```

# Creating issues

Anyone is welcome to create an issue to:

 - **report a bug.** In this case, please provide as much relevant information as possible to help us fix the bug.

 - **suggest an improvement**. In this case, please explain carefuly what is not working for you with wrfpp as is, and what will become possible with your improvement that was not possible before.

 - **ask for a new feature**. In this case, please explain carefuly why you think adding this feature is relevant for wrfpp, and suggest one or more usecase(s).

# Making a pull request

Before making a pull request, you must ensure that there exists a related issue. In other words, each pull request must be associated whith an existing issue. It is ok to have several pull requests associated with the same issue. The reverse is not ok. Create the issue if needed, following the instructions above.

If you are not a member of the [WRF-Chem-Polar organisation](https://github.com/WRF-Chem-Polar) with triage permissions, you must get approval on the issue from one of them before starting working on the corresponding pull request.

Create and do your work on a branch named `issue##/short-description-of-issue` where `##` is the issue number without leading zeros. If you have write access to the repository, you can create the branch there directly. Otherwise create it in your own fork.

Authors of pull requests are responsible for testing their code and making sure it works before requesting a review.

# Reviewing a pull request

Each pull request must obtain approval from one member of the [WRF-Chem-Polar organisation](https://github.com/WRF-Chem-Polar) with write privileges before it can be merged.

The guidelines for reviewing a pull request are:

 - Reviewers may, but do not have to, **test** the code.

 - Reviewers **must read the code**. They should request changes in the following circumstances:

   * clarity of the code can be improved.

   * the code can be simplified.

   * the code does not respect the wrfpp coding style (see below).

   * the code will fail in certain circumstances.

   * the code does not fully address the associated issue (or the sub-part of this issue that it is meant to address).

   * the code adds functionality or fix parts of the code that are beyond the scope of the associated issue. These should be treated in separate issues and pull requests.

 - Reviewers may have ideas for new features or interesting additions related to the pull request but that go beyong the scope of the original issue. In this case, the reviewer should create a separate issue instead of requesting the author to implement them.

# Versioning

We use version numbers formatted as major.minor. Each minor version will be git-tagged as such (eg. "v2.3"). Any commit in between two tagged minor or major versions will be tagged as a development version (".dev0") of the next minor version. For example, if the last tagged version is "v2.3", any subsequent commit until the next tagged version will use version "2.4.dev0". Only wrfpp maintainers may create stable versions and the associated tags.

# Coding style

The proposed Python code must respect the following:

 - Python's style guide described in [PEP8](https://peps.python.org/pep-0008/).

 - The format and quality controls imposed by [Ruff](https://docs.astral.sh/ruff/), according to the options defined in [pyproject.toml](./pyproject.toml). Note that a CI workflow will block any pull request that does not respect this.

 - The UK-vs-US English style guide defined [here](https://github.com/WRF-Chem-Polar/WRF-infra/issues/148).

# Derivative works

`wrfpp` is free and open-source software: you are welcome to mofify it, distribute it, and distribute modified versions of it, as long as you abide the (very few) requirements of the [BSD 3-clause license](./LICENSE). These are mostly requirements of attribution and of not using our names for promoting your derived products.
