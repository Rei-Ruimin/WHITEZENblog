# WHITEZENblog
A Static Blog for WHITEZEN

WHITEZENblog is a static blog created for my friend, WHITEZEN, to post her fanfiction. Please be advised that the content is NSFW and is in Chinese.

[Visit the blog](https://blog.whitezenblog.top/)

## Tutorial
### Setting Up Hexo, GitHub, Netlify, and Cloudflare

I followed [this guide](https://blog.cuijiacai.com/blog-building/) to get started. Essentially, I used Hexo to create the blog code and stored it on GitHub. Then, I used Netlify to deploy the blog online. To ensure the blog loads quickly in China, I utilized Cloudflare. The only modification I made to the guide was purchasing my domain name from NameSilo instead of the recommended provider, as it was more economical. NameSilo provides buttons that assist in setting up DNS and changing the nameserver, as illustrated below.

### Adding a CMS with hexo-netlify-cms

To incorporate a Content Management System (CMS) into the blog, I utilized the [hexo-netlify-cms package](https://www.npmjs.com/package/hexo-netlify-cms). If you follow the official guide, be aware that it defaults to using the 'master' branch instead of 'main' in your Git repository. To address this, I created a new 'master' branch for production, as suggested in [this discussion](https://answers.netlify.com/t/git-gateway-error/12220/19).

### Setting Up Comments with Waline, LeanCloud, Vercel

As I used the Redefine theme with Hexo, I followed its [official guide](https://redefine-docs.ohevan.com/posts/comment) to add comments. Since Vercel (the host) is not accessible in China, I used my own domain (whitezenblog.top). I configured the comment.whitezenblog.top CNAME DNS in NameSilo, added the domain to Cloudflare, and then specified comment.whitezenblog.top in Vercel as the comment server domain.

## Conclusion
That's it! Apart from waiting for DNS updates, you should be able to complete the setup in less than a day. This guide is designed to be straightforward and easy to follow, enabling you to establish your own blog with minimal hassle. Happy blogging!
