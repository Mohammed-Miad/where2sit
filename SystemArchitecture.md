where2sit Architecture

![High Level Component Diagram](high_level_component_diagram.png)

The system is organized into a browser based frontend, a Django backend, a SQLite database, and an external HTMX CDN dependency. Users interact through Django rendered HTML templates, which send page requests, form submissions, and AJAX/fetch calls to the Django application layer. On the backend, Django Auth handles login/session access control while the Rooms app views and models process room listing, reservations, favorites, and ratings using Django ORM. The backend reads and writes application data in SQLite, and the frontend also loads HTMX from CDN at runtime to support client-side interaction behavior.
