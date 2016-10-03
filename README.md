# Installation

Install using `pip`.

    pip install django-dutils

Add `dutils` to your `INSTALLED_APPS` setting.

    INSTALLED_APPS = (
        ...
        'dutils',
    }


# Usage

## Google Analytics

1.  Add your Google Analytics Tracking ID setting.

        # Example:
        GOOGLE_ANALYTICS_TRACKING_ID = 'UA-########-#'

2.  Load and use `google_analytics` templatetag in your template

        {% load google_analytics %}
        <html>
        <head>
            ...
            {% google_analytics %}
        </head>
        <body>
            ...
        </body>
        </html>

3.  __(Alternative step 2)__ import the template `dutils/google_analytics.html`
    if you are usinng the app_directory template loader installed.

        <html>
        <head>
            ...
            {% import "dutils/google_analytics.html" %}
        </head>
        <body>
            ...
        </body>
        </html>


