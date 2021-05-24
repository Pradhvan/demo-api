![](https://github.com/scanapi/design/raw/main/images/github-hero-dark.png)

# Demo API

This is an API built only for demo purposes of [ScanAPI](https://github.com/camilamaia/scanapi). It
can be accessed at https://demo.scanapi.dev/.


## Development

### How to run demo-api locally

> The setup process's prerequisites are [Python 3.6+](https://www.python.org/downloads/), [pip](https://pip.pypa.io/en/stable/installing/) and [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed in your system.

1. Fork scanapi/demo-api so you would get the repo in your github account such as *yourusername*/demo-api and clone the your Git repo.

```
git clone https://github.com/<your username>/demo-api.git
```

2. Create a new virtual environment and activate virtual environment.

* For creating virtual environment we are using the method mentioned in the Python Python documentation. Feel free to use any other library like [virtualenv](https://virtualenv.pypa.io/en/latest/) or [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) for creating a new environment.
```
python3 -m venv DemoAPI
source DemoAPI/bin/activate
```

3. Install the demo-api dependencies

```
cd demo-api
pip install -r requirements.txt
```

4. Make migrations and run the demo-api

```
python manage.py migrate
python manage.py runserver
```