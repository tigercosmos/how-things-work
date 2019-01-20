# Browsing Websites

The technology around us affects us profoundly - emotionally, behaviorally, cognitively. We could easily spend a paramount span to not only watch videos online but also browse websites on the internet every day. However, have you ever thought about how the websites work and what is the mechanism inside the box?

When we want to open a website, we will first launch a browser and enter some keywords to search via the search engine, which might be Google, providing you a list of websites relevant to the keywords; meanwhile, you would click one of them that catch your eyes. Though Google is indeed a website, I would like to explain how a website works via the one clicked by you. Say that the website is `Amazon.com`.

Once you click the link of `Amazon.com`, The browser will send information, called HTTP requests in computer terminology, to the server of Amazon, which is running on the domain of the link. Whenever the server receives requests from any clients, which the one is that of your browser in the computer or the smartphone, it replies with the website HTML file of Amazon, which is usually called `index.html`, the entry of the site, as an HTTP response. Then browser gets `index.html` of Amazon and starts the process of rendering it.

![first indext](https://user-images.githubusercontent.com/18013815/51441514-72d73e80-1d0d-11e9-876d-42dd6a6a7b0d.jpg)


While rendering the `index.html` file, the browser would probably find the file includes many other resources, such as CSS, JavaScript or media files. These files would be requested to the servers, which each file belongs to, such as a media file from the server located at `media.amazon.com` or the CSS file located at `www.amazon.com`. In summary, a website is composited by some files, but the client always receives the first file, and need to call for others files then.


![other resources](https://user-images.githubusercontent.com/18013815/51441515-72d73e80-1d0d-11e9-8cf4-a38742fcd492.jpg)

Now the browser gets all resources required to render the website. With a complex process including parsing HTML, JavaScript and CSS files, laying out the website components, rendering the elements of the page to pixels on the screen, we are able to see the website appearance of Amazon shown on the displayer.

tags: server, client, website, browser, software-engineering
