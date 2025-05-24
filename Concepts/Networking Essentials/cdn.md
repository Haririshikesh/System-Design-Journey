# Content Delivery Network (CDN)

A **Content Delivery Network (CDN)** is a geographically distributed group of servers that work together to provide fast delivery of internet content. Generally, static files such as HTML/CSS/JS, photos, and videos are served from a CDN.

## Why Use a CDN?

Using a CDN offers several significant benefits:

* **Increased Content Availability and Redundancy:** By distributing content across multiple servers, a CDN ensures that content remains available even if one server experiences issues.
* **Reduced Bandwidth Costs:** CDNs can offload traffic from your origin server, leading to lower bandwidth usage and associated costs.
* **Improved Security:** Many CDNs offer security features like DDoS protection and SSL/TLS encryption.
* **Enhanced Performance:** Users receive content from data centers close to them, significantly reducing latency and improving loading times. This also reduces the load on your origin servers.

## How Does a CDN Work?

In a CDN, the **origin server** contains the original versions of the content. **Edge servers**, also known as caching servers, are numerous and distributed across various locations around the world.

To minimize the distance between visitors and the website's server, a CDN stores a cached version of its content in multiple geographical locations known as **edge locations**. Each edge location contains several caching servers responsible for content delivery to visitors within its proximity.

Once static assets are cached on all the CDN servers for a particular location, all subsequent website visitor requests for these static assets will be delivered from these edge servers instead of the origin. This process drastically reduces the origin server's load and improves overall scalability.

**Example:** When someone in the UK requests a website hosted in the USA, they will be served from the closest edge location (e.g., a London edge location). This is much quicker than having the visitor make a complete request to the origin server, which would significantly increase latency.

## Types of CDNs

CDNs are generally divided into two main types based on how content is populated and updated:

### Push CDNs

In a Push CDN, you (the content provider) actively "push" new content to the CDN whenever changes occur on your server. You take full responsibility for providing content, uploading it directly to the CDN, and rewriting URLs to point to the CDN. You can configure when content expires and when it should be updated. Content is uploaded only when it is new or changed, minimizing traffic but potentially maximizing storage on the CDN.

* **Best for:** Sites with a small amount of traffic or sites where content isn't often updated. Content is placed on the CDNs once, instead of being re-pulled at regular intervals.

### Pull CDNs

In a Pull CDN, the cache is updated based on client requests. When a client sends a request for static assets that are to be fetched from the CDN, if the CDN doesn't have that specific asset in its cache or if its cached version is stale, it will "pull" the newly updated asset from the origin server. It then populates its cache with this new asset and serves it to the user.

* **Best for:** Sites with heavy traffic. This requires less maintenance because cache updates on CDN nodes are performed dynamically based on requests from the client. Traffic is spread out more evenly, with only recently-requested content remaining on the CDN.

## Disadvantages of CDNs

While CDNs offer numerous advantages, they also come with some potential drawbacks:

* **Extra Charges:** Using a CDN can be expensive, especially for high-traffic services, as costs often scale with data transfer and usage.
* **Restrictions/Blocking:** Some organizations or countries may block the domains or IP addresses of popular CDNs due to various reasons, which could hinder content delivery.
* **Location Dependency:** If the majority of your audience is located in a country where the CDN has no servers, the data on your website may have to travel further than without using any CDN, potentially negating the performance benefits.

## Examples of Widely Used CDNs

* Amazon CloudFront
* Google Cloud CDN
* Cloudflare CDN
* Fastly

---

## Key Takeaways

* CDNs improve website performance, availability, and security by distributing content geographically.
* They work by caching content on "edge servers" closer to users, reducing latency and origin server load.
* **Push CDNs** are better for less frequently updated content; content is pushed manually.
* **Pull CDNs** are better for high-traffic sites; content is pulled from the origin as needed.
* Consider costs, potential blocking, and server locations when choosing a CDN.