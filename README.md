<div align="center">
  <a href="http://netflix-clone-with-tmdb-using-react-mui.vercel.app/">
    <img src="./public/assets/netflix-logo.png" alt="Logo" width="100" height="32">
  </a>

  <h3 align="center">Netflix Clone</h3>

  <p align="center">
    <a href="https://netflix-clone-react-typescript.vercel.app/">View Demo</a>
    ·
    <a href="https://github.com/crazy-man22/netflix-clone-react-typescript/issues">Report Bug</a>
    ·
    <a href="https://github.com/crazy-man22/netflix-clone-react-typescript/issues">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#prerequests">Prerequests</a>
    </li>
    <li>
      <a href="#which-features-this-project-deals-with">Which features this project deals with</a>
    </li>
    <li><a href="#third-party-libraries-used-except-for-react-and-rtk">Third Party libraries used except for React and RTK</a></li>
    <li>
      <a href="#contact">Contact</a>
    </li>
  </ol>
</details>

<br />

<div align="center">
  <img src="./public/assets/home-page.png" alt="Logo" width="100%" height="100%">
  <p align="center">Home Page</p>
  <img src="./public/assets/mini-portal.png" alt="Logo" width="100%" height="100%">
  <p align="center">Mini Portal</p>
  <img src="./public/assets/detail-modal.png" alt="Logo" width="100%" height="100%">
  <p align="center">Detail Modal</p>
  <img src="./public/assets/grid-genre.png" alt="Logo" width="100%" height="100%">
  <p align="center">Grid Genre Page</p>
  <img src="./public/assets/watch.png" alt="Logo" width="100%" height="100%">
  <p align="center">Watch Page with customer contol bar</p>
</div>

## Prerequests

- Create an account if you don't have on [TMDB](https://www.themoviedb.org/).
  Because I use its free API to consume movie/tv data.
- And then follow the [documentation](https://developers.themoviedb.org/3/getting-started/introduction) to create API Key
- Finally, if you use v3 of TMDB API, create a file named `.env`, and copy and paste the content of `.env.example`.
  And then paste the API Key you just created.

## Which features this project deal with

- How to create and use [Custom Hooks](https://reactjs.org/docs/hooks-custom.html)
- How to use [Context](https://reactjs.org/docs/context.html) and its provider
- How to use lazy and Suspense for [Code-Splitting](https://reactjs.org/docs/code-splitting.html)
- How to use a new [lazy](https://reactrouter.com/en/main/route/lazy) feature of react-router to reduce bundle size.
- How to use data [loader](https://reactrouter.com/en/main/route/loader) of react-router, and how to use redux dispatch in the loader to fetch data before rendering component.
- How to use [Portal](https://reactjs.org/docs/portals.html)
- How to use [Fowarding Refs](https://reactjs.org/docs/forwarding-refs.html) to make components reusuable
- How to create and use [HOC](https://reactjs.org/docs/higher-order-components.html)
- How to customize default theme of [MUI](https://mui.com/)
- How to use [RTK](https://redux-toolkit.js.org/introduction/getting-started)
- How to use [RTK Query](https://redux-toolkit.js.org/rtk-query/overview)
- How to customize default classname of [MUI](https://mui.com/material-ui/experimental-api/classname-generator)
- Infinite Scrolling(using [Intersection Observer API](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API))
- How to make awesome carousel using [slick-carousel](https://react-slick.neostack.com)

## Third Party libraries used except for React and RTK

- [react-router-dom@v6.9](https://reactrouter.com/en/main)
- [MUI(Material UI)](https://mui.com/)
- [framer-motion](https://www.framer.com/docs/)
- [video.js](https://videojs.com)
- [react-slick](https://react-slick.neostack.com/)

## Install with Docker

```sh
docker build --build-arg TMDB_V3_API_KEY=your_api_key_here -t netflix-clone .

docker run --name netflix-clone-website --rm -d -p 80:80 netflix-clone
```

## Todo

- Make the animation of video card portal more similar to Netflix.
- Improve performance. I am using `context` and `provider` but all components subscribed to the context's value are re-rendered. These re-renders happen even if the part of the value is not used in render of the component. there are [several ways](https://blog.axlight.com/posts/4-options-to-prevent-extra-rerenders-with-react-context/) to prevent the re-renders from these behaviours. In addition to them, there may be several performance issues.
- Replace bundler([Vite](https://vitejs.dev/guide)) with [Turbopack](https://turbo.build/pack/docs/why-turbopack). Turbopack is introduced in Next.js conf recently. It's very fast but it's nor ready to use right now. it just support Next.js, and they plan to support all others as soon as possible. so if it's ready to use, replace [Vite](https://vitejs.dev/guide) with [Turbopack](https://turbo.build/pack/docs/why-turbopack).
- Add accessibilities for better UX.
- Add Tests.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

![sonar-1](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/f8f60cf2-7c5c-438b-8028-b61eb78ab9ff)

![pro-2](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/56de0807-ea0a-43ef-aaea-3249b2c8c250)

![pro-3](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/92c78fae-f507-41dc-8731-506ad2db4eb5)

![pro-4](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/05e08e59-ff03-4495-800e-07eb21d3c602)

![pro-5](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/fc1147c1-162f-4c14-a251-3f03c5348d29)

![pro-6](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/5e7fba38-de8e-4c43-a89d-af567ee6dbad)

![pro-7](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/e57e1299-10ae-4b46-969b-dbe156c6781b)

![pro-1](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/f7c1e3f7-2e81-4cfa-9b5a-57b39f69017e)

![gra-1](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/7999fa51-f3d8-4b39-b8cd-8dc539a38e60)

![Grafana-1](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/d26f7b7c-c9c2-4ef3-a77c-70ce047d94a1)

![firstJob-1](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/f5cbcfdb-285d-4766-b938-c1302b4886dd)

![grafana-jenkins-first](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/00e376dd-e6df-4784-bc8f-4244d0ec73a6)

![jenk-1](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/b0c24c1b-c6fc-42ac-88c8-21a02eaa04fa)

![jen-job-3](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/18b1d7f9-4667-4f25-9123-46e312dd1017)

![Output1](https://github.com/darjidhruv26/Netflix-clone/assets/90086813/c35223ad-137c-485a-b3f6-df324a2d0a97)
