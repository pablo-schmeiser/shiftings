# Development

## Development Setup

1. Clone the [repository](https://github.com/HaDiNet/shiftings) and navigate to the project directory.
2. Set up a Python virtual environment using `venv` and install dependencies listed in `pyproject.toml`.
3. Activate the virtual environment in a shell session by running `source venv/bin/activate` (Linux/Mac) or `venv\Scripts\activate` (Windows) or configure your IDE accordingly.
4. The default settings are configured for development (`DEBUG = True`). Adjust as needed in `src/shiftings/settings.py`.
5. Initialize the database using `setup_db.sh`, which runs migrations and loads example data fixtures.
6. Start the development server with `python src/manage.py runserver` and access the application at <http://127.0.0.1:8000/>.

**NOTE:** Pre-defined user fixtures are available for testing different access levels. Superuser: `bob`, Staff: `perry`. The users access levels are based on the TV series [Scrubs](https://en.wikipedia.org/wiki/Scrubs_(TV_series)).

## Upgrade and Deployment

- To upgrade Django, follow the official Django upgrade documentation and verify the setup with `python -W all src/manage.py check --deploy`.

For more information, refer to the project [README](https://github.com/HaDiNet/shiftings/blob/master/README.md) or the [official Django documentation](https://docs.djangoproject.com/).
