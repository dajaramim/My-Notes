# My-Notes

## Internet

### How does the internet Work?
The internet spans the globe through fiber optic cables. Data is transferred using light pulses that represent 0s and 1s.

To make the internet more organized and secure, there are protocols like TCP/IP, HTTP, SSL/TSL, and DNS.

There are computers called <strong>servers</strong> that store websites, databases, etc., and computers that make requests are called <strong>clients</strong>.

First, we need to understand what a packet is. A packet is like the atom of a resource on the internet. When we want to send a photo to a friend, my computer sends the photo in fragmented packets. When my friend's computer has every piece of my photo, the photo is reassembled. This way is more efficient than sending the whole photo in one go. Also, when a packet is missing, my computer is notified, so it sends the missing piece.

To establish a network, we use a computer connected to a router. The router knows where to send a packet and is connected to other routers, forming a global network connecting computers worldwide.

For determining where to send a packet, every computer connected to the internet has an address called an IP (Internet Protocol) address."

In summary, we transmit data in fragmented packets, where each packet comprises sequences of 0s and 1s conveyed as light pulses through fiber optic cables. This data is transmitted from a client to a server using various protocols, and the destination is determined by the IP address.

![Internet Image](images/network.webp)

### What is HTTP?
HTTP (Hypertext Transfer Protocol) is a protocol that allows the exchange of information through requests and responses between clients and servers. It is stateless, meaning that each HTTP request the server receives is independent and does not relate to requests that came before it.

HTTP has four methods: GET, POST, PUT, and DELETE.

A request or response is broken down into two main components: headers and body. The header contains information about the communication between the client and the server, such as the type of content, content-length, user-agent, cookies, authentication, and more.

The body contains the actual data, such as JSON or HTML.
![header and body http image](images/http-header-and-body.png)

When we make a request or receive a response, we always get a status code. The most common ones are 200, which means everything is okay, 404 for 'not found,' and 500 indicating an internal server error.

![status code image](images/statushttp.jpg)

### What is Domain Name?
The domain name of a website is the easy-to-remember address used instead of the IP, which is just a numerical representation.

![Domain image](images/url-structure.webp)

### What is Hosting?
Hosting is an online service that allows us to publish websites on the internet.

There are different types of hosting, such as Shared Hosting, VPS Hosting, and Dedicated Servers.

Shared Hosting: In this setup, we share the same computer resources, including RAM and CPU, with other websites. While this option is more cost-effective, it may not be ideal if our website experiences heavy traffic and requires more resources.

Virtual Private Server (VPS): In this type of hosting, a single physical server hosts multiple virtual servers. Each virtual server operates independently, allowing users to have their own isolated server environment within the larger physical server. The advantage of this is that we can obtain the precise resources we need, such as a specific amount of RAM, processing power, storage, and bandwidth.

Dedicated Servers: This option involves having a server exclusively for my use, which can be quite expensive.

### DNS
The Domain Name System is a distributed and decentralized database that contains the domain names of websites along with their corresponding IP addresses.

### What is a Browser
A browser is software that enables us to navigate through the web, such as Firefox, Chrome, Safari, etc.

## HTML
HTML is the backbone of a webpage, providing the structure where we can place headings, text, images, videos, etc.

HTML has a variety of tags, including:

- `<html></html>` which serves as the root of the document.
- `<head></head>` containing machine-readable information (metadata) about the document.
- `<title></title>` representing the title of the webpage.
- `<body></body>`  indicating the content of the document.
- `<div></div>`  serving as a container for flow content.
- `<p></p>` used for paragraphs.

There are many more tags, in the link below.

[Documentation HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

### Semantic
We can create better-organized, more search engine-friendly, and more accessible HTML using the following tags:
- `<header>` for the top section of the webpage.
- `<nav>`  this section contains navigation links.
- `<main>` this is the section most important of the webpage.
- `<article>` this is for an independent piece of content.
- `<aside>` this is a sidebar typically used for supplementary      information, advertisements, or related articles.
- `<section>` this tag is used to mark up sections that are thematically related or to break down a theme into different parts.
- `<footer>` this tag is used to define the footer section of a webpage, typically containing elements such as copyright information, contact details, or social media links.
- `<details>` and `<summary>` are used to make a collapsible section of content.
  Example of details and summary.

    ```
    <details>
        <summary>Click to expand</summary>
        <p>Content goes here</p>
    </details> 
    ```
  
- `<figure>` and `<figcaption>`  are tags used to include visual content within a document, along with a caption that references the image or visual content. 
     ```
    <figure>
        <img src="image.jpg" alt="Image description" />
        <figcaption>Image caption</figcaption>
    </figure>
    ```
- `<mark>` this tag is used to mark up text that has been highlighted for some reason

    ```
    <p>Here is some <mark>highlighted</mark> text.</p>
    ```
    <p>Here is some <mark>highlighted</mark> text.</p>

- `<time>` this tag is used to mark up date or time
- `<progress>` this tag is used to mark up a progress bar
  
  ```
  <progress value="50" max="100"></progress>
  ```
  <progress value="50" max="100"></progress>

### Good Practices
1. Use only one `<h1>` per document.
2. Don't skip heading levels. If you use `<h2>`, then don't use  `<h4>` right after.
3. Use `<figure>` and `<figcaption>` to add captions to an image.
4. Do not use divs to create semantic tags like header or footer.
5. Avoid using `<b>` and `<i>` for bolding or italics. Prefer `<strong>` and `<em>`.
6. Don't place block-level elements within inline elements.


## Computer Science