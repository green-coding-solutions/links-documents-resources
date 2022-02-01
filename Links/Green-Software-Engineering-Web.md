## Basic / Overview
- https://principles.green/ - A general list with categorys and concepts. Very unspecific and not too dense in information, but often used as link, so we include it here for completeness
- https://docs.microsoft.com/de-de/learn/modules/sustainable-software-engineering-overview/ - Good overview but not many details
  => Most important part is that finally someone orders the relevancy of network related carbon emission: https://docs.microsoft.com/de-de/learn/modules/sustainable-software-engineering-overview/8-network-efficiency


## Calculation models
- https://theshiftproject.org/en/article/lean-ict-our-new-report/ - 1-Byte model to generally quantify and compare different digital services in terms of carbon emission
But they base their calculations a lot on this study: https://www.mdpi.com/2078-1547/6/1/117/htm?utm_source=morning_brew 
Part 4 in particular! However. They also reference to other studies for calculations of network electricity consumptions: [91,92,93,94 ...] in Article references.
Most not free and not on sci-hub. Others very impractical, cause they do not segment into hops, which would be very helpful. And they also do not provide idle consumption averages of devices, which makes given formulas useless on their own.
- https://greensoftware.foundation/articles/gps-up-a-better-metric-for-comparing-software-energy-efficiency - The "Green Up" metric. Instead of Speed-Up or Power-Down

## Green Hosting
- https://www.wholegraindigital.com/blog/choose-a-green-web-host/
- https://www.thegreenwebfoundation.org/ - Check Green Hosting
- https://blog.cloudflare.com/green-hosting-with-cloudflare-pages/


## Bot Blocking to reduce server load
- https://github.com/mitchellkrogza/apache-ultimate-bad-bot-blocker/tree/master/Apache_2.4

## Things everyone knows, that do not need a link:
- Lazy Loading
- Minifiying
- Caching. But yeah .... nobody caches! This means DB-requests .... but also NGINX cache which is very easy to set up. 
- gzip (I was unsure at first, but to unpack the compression is no match for 5-10 hops of servers copying the vast amounts of data)
- webp & Avif - https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types#avif_image
- Responsive images. As well in dpi, as in width / height
- Use HTTP2 / HTTP3

## Website Carbon Calculators
- https://ecograder.com/results#green-hosting
- https://digitalbeacon.co/report/zeit-de
- https://www.websitecarbon.com/website/zeit-de-index/
- https://www.climatecare.org/calculator/
- https://github.com/thegreenwebfoundation/co2.js
- https://ecologi.com/krystal
- https://mobile-efficiency-index.com/en/ - Includes mobile device power consumption

## Practical Coding Resources and Snippets
- https://sustywp.com/ - Very low carbon intense Wordpress templates directory
- https://csaba.blog/global-warning-a-wordpress-blog-with-a-tiny-footprint/ - Low Carbon Wordpress template
- https://greentheweb.com/my-website-relaunch-with-an-amazing-score-0-1g-co2-page-view/ - Walktrough for Template Optimization
- https://the-sustainable.dev/resources/ - Free resource directory with Wordpress snippets, emoji removal, API best-practices etc. (requires free  registration)
- https://withcabin.com/ - Low carbon Google Analytics Alternative
- https://sustainablewebdesign.org/category/development - Best practices Checklist
- https://nachhaltiges-webdesign.jetzt/ - Best practices directory

## Power Grid Energy Source
- https://app.electricitymap.org/zone/DK-DK1 - See if energy is currently renewable or from coal etc. for your location

## Cloud Carbon Impact Calculator
- https://appsource.microsoft.com/en-us/product/power-bi/coi-sustainability.emissions_impact_dashboard?tab=Overview
- https://mlco2.github.io/impact/

## Funding / Partnership
- https://greensoftware.foundation/working-groups/innovation
- https://climaccelerator.climate-kic.org/

## SDKs
- https://github.com/Green-Software-Foundation/carbon-aware-sdk/tree/dev/carbon-aware-sdk - Not ready yet :(
- https://github.com/mlco2/codecarbon - Track code runtime / ressource-usage carbon equivalents

## Personal Non-Web Carbon Calculator
- https://uba.co2-rechner.de/en_GB/

## Browser Carbon usage through web-surfing
- https://microsoftedge.microsoft.com/addons/detail/wedeex/jbocoolinibenmobjadejejdbanalfee
- https://github.com/carbonalyser/Carbonalyser


## EU Plans
- https://sdialliance.org/roadmap
