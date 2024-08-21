# API with Swagger

## Description
This directory contains API files and documentation for a web application. The API is built using Flask and documented with Swagger.

## Environment

* **OS:** Ubuntu 14.04 LTS
* **Language:** Python 3.4.3
* **Application Server:** Flask 0.12.2, Jinja2 2.9.6
* **Web Server Gateway:** gunicorn (version 19.7.1)
* **Database:** MySQL Ver 14.14 Distrib 5.7.18
* **Documentation:** Swagger (flasgger==0.6.6)
* **Style:**
  * **Python:** PEP 8 (v. 1.7.0)

## Testing API

To run the API and test it:

1. **Execute the program:**

   ```bash
   HBNB_MYSQL_USER=hbnb_dev HBNB_MYSQL_PWD=hbnb_dev_pwd \
   HBNB_MYSQL_HOST=localhost HBNB_MYSQL_DB=hbnb_dev_db HBNB_TYPE_STORAGE=db \
   HBNB_API_HOST=0.0.0.0 HBNB_API_PORT=5000 python3 -m api.v1.app
   ```

2. **Testing with Swagger:**

   * Open your browser and visit the path: `/apidocs` or:
   * For localhost: `http://0.0.0.0:5000/apidocs`
   * For your domain: `http://yourdomain/apidocs`

3. **Testing from CLI:**

   Use the `curl` command to make API requests.

   Example:

   ```bash
   curl -X GET http://0.0.0.0:5000/api/v1/states/
   ```

This will allow you to interact with the API and view the Swagger documentation for available endpoints.
