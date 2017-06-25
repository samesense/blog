+++
title = "my python project structure template"
date = 2017-06-25T10:08:24-04:00
draft = false
+++

[Cookiecutter](https://github.com/audreyr/cookiecutter) allows you to setup a
project's structure from templates. I use a
modified
[data science cookiecutter template](http://drivendata.github.io/cookiecutter-data-science/),
found [here](https://github.com/samesense/cookiecutter-data-science). The
benefits of a project template
are
[better described by others](http://drivendata.github.io/cookiecutter-data-science/).
I use one for consistent navigation across projects, and to save configuration
time.

My modifications to the [data science template](https://github.com/drivendata/cookiecutter-data-science) are below.
* I add a work directory to hold analysis results and summaries that do not belong in reports.
* I add a log directory to hold log output from programs like STAR and snpeff
* I add a tests directory under src/ to hold unit tests, and a tests directory under data/ to hold testing data.
* I replace the Makefile with a snakefile sf.py, in src/rules. This is controled
  by run.sh. Associated rules and constants are stored in src/rules/. My
  snakefile is setup to send me an SMS when the pipeline completes. To use this
  feature, change the [twilio](https://www.twilio.com) keys in
  SECRETS/pass_wd.py
  (look
  [here](https://github.com/samesense/cookiecutter-data-science/blob/master/%7B%7B%20cookiecutter.repo_name%20%7D%7D/src/rules/const.py)).



