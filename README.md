# My NL-RSE19 slides

- Title: Creating a community of contributors for scientific open-source projects: The preCICE case
- Speaker: Gerasimos Chourdakis, Technical University of Munich
- Authors: Gerasimos Chourdakis, Benjamin Uekermann, + [more](https://www.precice.org/about/)
- Event: [NL-RSE19](https://nl-rse.org/events/NL-RSE19.html), Amsterdam, The Netherlands
- Date: November 20, 2019

[Start the presentation](https://makish.github.io/nlrse19-slides/) - [Get the PDF](export/nlrse19-chourdakis.pdf)

## Abstract

Contributors are vital for open-source projects and users are essential for a scientific project to have impact in society. Still, scientific projects often suffer from low visibility and trust, while only the core developers contribute.

Getting (the right) users is a very fulfilling, yet long trip. Turning them further into motivated contributors is even harder, but can be invaluable for the project's sustainability. From getting the first user to establishing a self-sustained community, it is essential for a project to provide continuous user support, low communication barrier, and active development. However, as the community grows, it also needs to function in a scalable, distributed way.

On the technical side, splitting a project into components that can isolate any "damage" and establishing a reliable testing infrastructure can increase the confidence of new contributors. With a detailed code reviewing culture and brave integration into the project, these contributors can further turn to senior maintainers.

Having a strong backbone in high-performance computing and multi-physics simulations, preCICE now needs additional expertise to adapt to a growing number of users. This talk will present our findings on developing a project with isolated components, our exploration of different communication channels, and the many benefits and challenges that a diverse community can bring to scientific projects.

## Build

Follow the instructions on [reveal.js](https://github.com/hakimel/reveal.js/tree/33bed47daca3f08c396215415e6ece005970734a), or just install Node.js 4.0.0 or later and do:

```bash
npm install
npm start
```

and go to [localhost:8000](http://localhost:8000/) to see the slides.

## Convert to PDF

See section "[Export to PDF](https://github.com/hakimel/reveal.js/tree/33bed47daca3f08c396215415e6ece005970734a#pdf-export)" in the reveal.js README.

[Decktape](https://github.com/astefanutti/decktape) does a marvelous job converting this presentation to PDF, even the chart.js plots. Get the Docker image (see Decktape README) and run (for localhost):

```bash
docker run --rm -t --net=host -v `pwd`:/slides astefanutti/decktape -s 1024x768 http://localhost:8000 slides.pdf
```

## License & more

- License: [CreativeCommons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
- Based on [reveal.js](https://github.com/hakimel/reveal.js). Template based on the "White" template by Hakim El Hattab.
- Also using the [Chart.js](https://www.chartjs.org/) extension.
- The TUM Logo is part of the Corporate Identity of the Technical University of Munich.

