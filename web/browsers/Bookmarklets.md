# Bookmarklets
I run my bookmarklets from KM like so :

![](https://i.imgur.com/UIQNrjr.png)

Here are the bookmarklets I use : 

## Go to first commit of currently open repo
\`\`\`Javascript
javascript:(b=\>fetch('https://api.github.com/repos/'+b[1]+'/commits?sha='+(b[2]||'')).then(c=\>Promise.all([c.headers.get('link'),c.json()])).then(c=\>{if(c[0]){var d=c[0].split(',')[1].split(';')[0].slice(2,-1);return fetch(d).then(e=\>e.json())}return c[1]}).then(c=\>c.pop().html\_url).then(c=\>window.location=c))(window.location.pathname.match(/\/([^\/]+\/[^\/]+)(?:\/tree\/([^\/]+))?/));
\`\`\`

## [Online article discussion finder](https://github.com/theoretick/discuss-it)

Lets you see where the link you are watching right now has been discussed before. Super handy.