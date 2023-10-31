# Onsite Support QR Landing Page

[![QR Landing Template](media/qr-landing-demo-04.png)](https://qrlanding.netlify.app/)

[Demo](https://qrlanding.netlify.app/) | [Documentation](https://support.onsitesupport.io/) | [Website](https://onsitesupport.io/)

## Overview

A front-end landing page prototype created as an option for [Onsite Support](https://onsitesupport.io/) customers. This has a "mobile-only" approach that focuses on a specific product to—highlight features, information, or registration options. This package would not require the need to develop a responsive soulution for larger screens since the content has been streamlined to a few items, actions grouped, and the minimal UI allows you clearly view the hero media.

## Performance Audits

<img src="media/with-autoplay-performance.png" width="350" alt="current Lighthouse performance audit scores" />
We are taking performance hits by using YouTube as our video source. Embedding video without third-party bloat is ideal. Either way, we should create a [`facade`](https://developer.chrome.com/docs/lighthouse/performance/third-party-facades/) to help limit the amount of code needed for first paint. We see some gains when we add `loading=lazy` & remove `autoplay`.

[Video Autoplay](https://qrlanding.netlify.app/](https://qrlanding.netlify.app/perf/autoplay)) | [No Autoplay](https://support.onsitesupport.io/](https://qrlanding.netlify.app/perf/no-autoplay))


## How to use

```sh
git clone https://github.com/ericthayer/qr-landing.git
cd qr-landing/
npm install
npm start
```

## markup

`index.html`

## styles

`scss/styles.scss`

### run to compile css

```sh
npm build
```

### result

`css/styles.css`
