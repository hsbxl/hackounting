# Hackounting

Tools for analysing Finances of HSBXL

## Usage

### 1. Data

Copy the `bank/` folder that contains all bank transfers in CSV
in the current directory, then run the notebook. If you do not have access to
the bank statements, copy the folder `bank-example/` to `bank/` and use the
example data inside.

### 2. Running the notebook

Reports are generated using [IPython Notebook](http://ipython.org/notebook.html).
Install it, preferably via [pip](https://docs.python.org/3/installing/).

```bash
pip install "ipython[notebook]"
```

Then, run the following command from within the repository to launch IPython
Notebook, and open the notebook.

```bash
ipython notebook
```

Pressing `Shift+Enter` after clicking on a cell executes its content, and
displays the output below if any.

### 3. Contributing to the notebook

These notebooks handle private information from the members. Before any commit,
make sure that none of the notebooks contains any personal data, and make sure
that all cell output is cleared (`Menu > Cell > All Output > Clear`).

Then generate an HTML output of the notebook for people who cannot run the
notebook using the following command, and commit both files:

```bash
jupyter-nbconvert HSBXL_Membership.ipynb
```

### 4. Sharing the results of the notebook

We plan to setup automatic builds of the reports online, but in the meantime
the best way to share the results is simply to post the generated HTML on the
[Mailing-List](https://hackerspace.be/Mailing_list).
