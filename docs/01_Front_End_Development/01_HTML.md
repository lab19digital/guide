You should keep your HTML bloat-free by using partials wherever possible. Using a templating language like Twig can help to keep your code clean and DRY. Twig pairs especially well with Wordpress using the Timber plugin. 

Any content that may be dynamic (integrated into Wordpress CMS), should be kept as a variable and passed into the partial using Twig's variable methods (like set). You should hard-code the variable's value but not the value in the HTML itself. You should assume that *most if not all* of the content will be dynamic, especially when it comes to a site that has i8ln. 

If you are developing for a different server-side platform, always prefer a templating language over raw HTML, as it allows you to keep your code slim and maintainable.