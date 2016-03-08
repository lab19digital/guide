Here is an overview of configuration and best practices with plugins:

1. Create a set of different environment variables inside wp-config, e.g. using htaccess or server variables, allowing smoother deployment
2. Implement [Twig/Timber](https://wordpress.org/plugins/timber-library/) to inject your logic into templates cleanly and to allow for a more modular build.
3. Implement [ACF](https://wordpress.org/plugins/advanced-custom-fields/) for any custom field requirements
4. Use named templates so that you can assign custom fields to specific templates
5. Use global options for ACF where necessary
6. If your functions file is destined to become bloated, split this up in components
7. Preserve as much Wordpress functionality as possible, for example, enqueue assets rather than hard-coding them
8. Delete unused themes (like 2014/2015/2016) to prevent bloat
9. Document custom fields (ACF), using labels and descriptions, so the CMS user understands where content goes
10. Hide the editor if it's not in use (option on ACF)
11. Install [Yoast](https://wordpress.org/plugins/wordpress-seo/) for SEO
12. Store API or other permanent details inside wp-config as constants

Use and contribute to our boilerplate [https://github.com/lab19digital/wp19](https://github.com/lab19digital/wp19) for local development as it comes automatically bootstrapped with much of what is listed above and installs all the latest dependencies from scratch.

There is a plethora of documentation on the web about best practices for further reading.