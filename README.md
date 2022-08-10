<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT LOGO -->
<br />
<div align="center">

<div align="center">
  <a href="https://github.com/gipplab/cs-insights-backend/issues"><img src="https://img.shields.io/github/issues/gipplab/cs-insights-backend.svg?style=for-the-badge"/></a>
  <a href="https://github.com/gipplab/cs-insights-backend/graphs/contributors"><img src="https://img.shields.io/github/contributors/gipplab/cs-insights-backend.svg?style=for-the-badge"/></a>
  <a href="https://github.com/gipplab/cs-insights-backend/stargazers"><img src="https://img.shields.io/github/stars/gipplab/cs-insights-backend.svg?style=for-the-badge"/></a>
  <a href="https://github.com/gipplab/cs-insights-main/blob/master/LICENSE"><img src="https://img.shields.io/github/license/gipplab/cs-insights-main.svg?style=for-the-badge"/></a>
  </div>
    <a href="https://github.com/gipplab/cs-insights-frontend"><img src="https://img.shields.io/badge/GitHub-Frontend-green?style=for-the-badge"/></a>
    <a href="https://github.com/gipplab/cs-insights-backend"><img src="https://img.shields.io/badge/GitHub-Backend-green?style=for-the-badge"/></a>
    <a href="https://github.com/gipplab/cs-insights-crawler"><img src="https://img.shields.io/badge/GitHub-Crawler-green?style=for-the-badge"/></a>
    <a href="https://github.com/gipplab/cs-insights-prediction-endpoint"><img src="https://img.shields.io/badge/GitHub-Prediction_Endpoint-green?style=for-the-badge"/></a>
  <div align="center">
  <p align="center">
    <br/>
    The main controller for services in the cs-insights project through docker-compose
    <br/>
  </p>
  <a href="https://github.com/gipplab/cs-insights-main">
    <img src="images/logo.jpg" alt="Logo" width="250">
  </a>
  <br/>
  <br/>
  <a href="https://jan-philip-wahle.gitbook.io/cs-insights/"><strong>Explore the docs »</strong></a>
  <br />
  <br />
  <a href="http://cs-insights.uni-goettingen.de/">View Demo</a>
  ·
  <a href="https://github.com/gipplab/cs-insights-main/issues/new?assignees=&labels=&template=bug_report.md&title=">Report Bug</a>
  ·
  <a href="https://github.com/gipplab/cs-insights-main/issues/new?assignees=&labels=&template=feature_request.md&title=">Request Feature</a>
  </div>

<br/>
<br/>
Demo Credentials <br/>
user: demo@cs-insights.com <br/>
password: demo

</div>

<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://cs-insights.uni-goettingen.de)

This project focusses on making information about computer science research available with a few mouse clicks. Therefore, we use the [DBLP Discovery Dataset D3](https://arxiv.org/abs/2204.13384) to show trends in volume, topics, impact, and many more.
The [frontend](https://github.com/gipplab/cs-insights-frontend) enables abstract access to the data through visualizations and filters. The [backend](https://github.com/gipplab/cs-insights-backend) enables access to the data through a well-defined REST API and makes it easy to index new data as well. The [prediction-endpoint](https://github.com/gipplab/cs-insights-prediction-endpoint) does the heavy lifting for analyzing topics and other semantic features using parents and childrens of docker containers that can run on different servers. Finally, the [crawler](https://github.com/gipplab/cs-insights-crawler) makes sure that the latest data is retrieved from the web, parsed, and stored into the backend.

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

[![React][React.js]][React-url]
[![Node][Passport]][Passport-url]
[![Node][Swagger]][Swagger-url]
[![Node][Express]][Express-url]
[![Node][Material.ui]][Material-url]
[![Node][Node.js]][Node-url]
[![Node][MongoDB]][Mongo-url]
[![Node][Docker]][Docker-url]


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started
To get a local copy up and running follow these simple example steps. The project relies on a singe docker-compose.yml file that is used to develop and deploy all the services.

### Prerequisites

You need to have `docker` and `docker-compose` installed.

### Installation

First, export the environment variables for the project.

```bash
set -o allexport
source .env
```

To start the development environment, run the following command:

```sh
docker-compose -f docker-compose.dev.yml up --build
```

This will start each service (e.g., backend, frontend) in development mode with hot reload. Whenever you change any files of the sub-repositories (e.g., ./cs-insights-frontend/src/App.tsx) the development server will reload and show the new rendered frontend.

To run the production environment in detached mode, run the following command:

```sh
docker-compose up -d
```

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage

The services are available on the following ports:
- frontend: `80`
- backend: `3000`
- prediction-endpoint: `4000`

_For more examples, please refer to the [Documentation](https://jan-philip-wahle.gitbook.io/cs-insights/) or the individual API documentation for [backend](https://gipplab.github.io/cs-insights-backend/), [frontend](https://gipplab.github.io/cs-insights-frontend/), [prediction-endpoint](https://gipplab.github.io/cs-insights-prediction-endpoint/), and [crawler](https://gipplab.github.io/cs-insights-crawler/)_.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

See the [project board](https://github.com/orgs/gipplab/projects/8) for a full list of features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
6. We will get in touch and include your feature in the next release.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Jan Philip Wahle - [@jan_wahle](https://twitter.com/jan_wahle) - wahle@gipplab.org
Terry Ruas - [@ruasterry](https://twitter.com/jan_wahle) - ruas@gipplab.org

Project Link: [https://github.com/gipplab/cs-insights-main](https://github.com/gipplab/cs-insights-main)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[product-screenshot]: images/system-overview.png
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Node.js]: https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white
[Node-url]: https://nodejs.org/en/
[Material.ui]:https://img.shields.io/static/v1?style=for-the-badge&message=Material+Design&color=757575&logo=Material+Design&logoColor=FFFFFF&label=
[Material-url]: https://mui.com/
[MongoDB]: https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white
[Mongo-url]: https://www.mongodb.com/
[Docker]: https://img.shields.io/static/v1?style=for-the-badge&message=Docker&color=2496ED&logo=Docker&logoColor=FFFFFF&label=
[Docker-url]: https://www.docker.com/
[Passport]: https://img.shields.io/static/v1?style=for-the-badge&message=Passport&color=222222&logo=Passport&logoColor=34E27A&label=
[Passport-url]: https://www.passportjs.org/
[Swagger]: https://img.shields.io/static/v1?style=for-the-badge&message=Swagger&color=222222&logo=Swagger&logoColor=85EA2D&label=
[Swagger-url]: https://swagger.io/
[Express]: https://img.shields.io/static/v1?style=for-the-badge&message=Express&color=000000&logo=Express&logoColor=FFFFFF&label=
[Express-url]: https://expressjs.com/
