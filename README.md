<p align="center">
  <a href="https://www.chartjs.org/" target="_blank">
    <img src="https://www.chartjs.org/media/logo-title.svg" alt="https://www.chartjs.org/"><br/>
  </a>
    Simple yet flexible JavaScript charting for designers & developers
</p>

<p align="center">
    <a href="https://www.chartjs.org/docs/latest/getting-started/installation.html"><img src="https://img.shields.io/github/release/chartjs/Chart.js.svg?style=flat-square&maxAge=600" alt="Downloads"></a>
    <a href="https://github.com/chartjs/Chart.js/actions?query=workflow%3ACI+branch%3Amaster"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/chartjs/Chart.js/ci.yml?branch=master&style=flat-square"></a>
    <a href="https://coveralls.io/github/chartjs/Chart.js?branch=master"><img src="https://img.shields.io/coveralls/chartjs/Chart.js.svg?style=flat-square&maxAge=600" alt="Coverage"></a>
    <a href="https://github.com/chartjs/awesome"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
    <a href="https://discord.gg/HxEguTK6av"><img src="https://img.shields.io/badge/discord-chartjs-blue?style=flat-square&maxAge=3600" alt="Discord"></a>
</p>

## Documentation

All the links point to the new version 4 of the lib.

* [Introduction](https://www.chartjs.org/docs/latest/)
* [Getting Started](https://www.chartjs.org/docs/latest/getting-started/index)
* [General](https://www.chartjs.org/docs/latest/general/data-structures)
* [Configuration](https://www.chartjs.org/docs/latest/configuration/index)
* [Charts](https://www.chartjs.org/docs/latest/charts/line)
* [Axes](https://www.chartjs.org/docs/latest/axes/index)
* [Developers](https://www.chartjs.org/docs/latest/developers/index)
* [Popular Extensions](https://github.com/chartjs/awesome)
* [Samples](https://www.chartjs.org/samples/)

In case you are looking for an older version of the docs, you will have to specify the specific version in the url like this: [https://www.chartjs.org/docs/2.9.4/](https://www.chartjs.org/docs/2.9.4/)

##A simple chart usage example
# Chart.js Bar Chart Example

This is a simple example of how to create a bar chart using Chart.js. In this example, we'll create a basic bar chart to visualize data.

## Prerequisites

Before you begin, ensure you have the following:

- A web browser to view the chart.
- Internet connectivity to load Chart.js from a CDN.

## Getting Started

To view the bar chart, follow these steps:

1. Create an HTML file (e.g., `index.html`) and paste the following code:

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <title>Chart.js Bar Chart Example</title>
       <!-- Include Chart.js library -->
       <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
   </head>
   <body>
       <!-- Create a canvas element to render the chart -->
       <canvas id="myChart"></canvas>

       <script>
           const ctx = document.getElementById('myChart');

           new Chart(ctx, {
               type: 'bar',
               data: {
                   labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
                   datasets: [{
                       label: '# of Votes',
                       data: [12, 19, 3, 5, 2, 3],
                       borderWidth: 1
                   }]
               },
               options: {
                   scales: {
                       y: {
                           beginAtZero: true
                       }
                   }
               }
           });
       </script>
   </body>
   </html>

## Configuration Options

Chart.js provides a wide range of configuration options that allow you to customize the appearance and behavior of your charts. Below is a list of common configuration options and their descriptions:

### Type of Chart

- **Option Name**: `type`
- **Description**: Specifies the type of chart to create (e.g., bar, line, pie).
- **Example**: To create a bar chart, set `type: 'bar'`.

### Data

- **Option Name**: `data`
- **Description**: Provides data for the chart, including labels and datasets.
- **Example**:

```javascript
data: {
    labels: ['Label1', 'Label2', 'Label3'],
    datasets: [{
        label: 'Dataset 1',
        data: [10, 20, 30],
        backgroundColor: 'rgba(75, 192, 192, 0.2)',
        borderColor: 'rgba(75, 192, 192, 1)',
        borderWidth: 1
    }]
}
```
## Contributing

Instructions on building and testing Chart.js can be found in [the documentation](https://www.chartjs.org/docs/master/developers/contributing.html#building-and-testing). Before submitting an issue or a pull request, please take a moment to look over the [contributing guidelines](https://www.chartjs.org/docs/master/developers/contributing) first. For support, please post questions on [Stack Overflow](https://stackoverflow.com/questions/tagged/chart.js) with the `chart.js` tag.

## License

Chart.js is available under the [MIT license](LICENSE.md).
