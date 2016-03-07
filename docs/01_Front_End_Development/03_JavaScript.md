JavaScript can easily become bloated if you're working in a single file and the project is particularly large. You may want to begin by using an AMD/CommonJS implementation so that you can separate out components easily into different files. Using webpack you can pack up these modules during development into browser-friendly JavaScript that can also be minified. If you read the next article, we briefly cover how you can accomplish this configuration by using Gulp or Grunt for your local development environment.

> For dependencies make sure you use package management like Bower or NPM

**What about JavaScript conventions?** Well much of your JavaScript will be handled mostly by jQuery plugins. Where any vanilla JavaScript may be written, ensure that you don't pollute the namespace. Make sure you pass jQuery using a closure.

	(function( $ ){
	  $( document ).ready( function(){ });
	})( jQuery );

If you're working in a single file, you'll definitely want to store all your methods in an object literal so that it's obvious to access them and your code is DRY. You can make use of the module pattern for this:

[https://toddmotto.com/mastering-the-module-pattern/](https://toddmotto.com/mastering-the-module-pattern/)

But I'd also encourage you to separate your files into modules to keep the codebase clean and intuitive.

	window.Module = ( function( $ ){
	 var self = {
	  ready : function(){
	   this.bind();
	  },
	  windowLoad : function(){},
	    bind : function(){}
	  };

	  $( function(){ self.ready(); })

      return {
       publicMethod : function(){}
      };
	})( jQuery );

