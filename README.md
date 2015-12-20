# LaTeX---My-header-file
This is the basic header file that I insert in most of my LaTeX projects

## To use it
```
\input{headers}

\begin{document}
%Your content comes here
\end{document}
```

It include some basics packages that I use a lot, like:
- babel (configured in english here)
- graphicx
- [url](http://ctan.org/pkg/url)
- [todonotes](https://github.com/henrikmidtiby/todonotes)
- [listings](https://en.wikibooks.org/wiki/LaTeX/Source_Code_Listings)

For the listing package, it declares explicitly the *JavaScript* langage.

## To insert a todo
```LaTeX
\todo[inline]{TODO here}
```

## To insert JavaScript code
```JavaScript
\begin{lstlisting}[language=JavaScript]
it('should redirect to the admin page', function(){
   	 var email = element(by.id('email-id')).sendKeys('b@b.com');
   	 var password = element(by.id('password-id')).sendKeys('123456');
	 var submit = element(by.id('connection'));
	 submit.click();
   	 expect(
   	 	browser.getCurrentUrl()
   	 ).toEqual('http://localhost:3000/#/admin/list-staffs');
   });
\end{lstlisting}
```
