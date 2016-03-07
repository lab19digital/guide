Here is an overview of some best practices (and their associated plugins) in Wordpress:

1. Implement [Twig/Timber](https://wordpress.org/plugins/timber-library/) to inject your logic into templates cleanly and to allow for a more modular build.
2. Implement [ACF](https://wordpress.org/plugins/advanced-custom-fields/) for any custom field requirements
3. Use named templates so that you can assign custom fields to specific templates
4. Use global options for ACF where necessary
5. If your functions file is destined to become bloated, split this up in components
6. Preserve as much Wordpress functionality as possible, for example, enqueue assets rather than hard-coding them
7. Delete unused themes (like 2014/2015/2016) to prevent bloat
8. Document custom fields (ACF), using labels and descriptions, so the CMS user understands where content goes
9. Hide the editor if it's not in use (option on ACF)
10. Install [Yoast](https://wordpress.org/plugins/wordpress-seo/) for SEO

Use and contribute to our boilerplate [https://github.com/lab19digital/wp19](https://github.com/lab19digital/wp19) for local development as it comes automatically bootstrapped with much of what is listed above and installs all the latest dependencies from scratch.

There is a plethora of documentation on the web about best practices for further reading.