## Personal Website 
<div align="center">
  Eneida Likaj
</div>

<div align="center">
  (509) 200-5084 * likaje@whitman.edu * https://www.linkedin.com/in/eneida-likaj-a7b257191/ 
  <p><a href="https://drive.google.com/file/d/1UC0yQGDHgcBRNg2DVpymw41IlIg1vByu/view?usp=sharing" target="_blank">Resume</a></p>
</div>

## Where's Schueller?
One of my major projects involved transforming Google location data from Prof. Schueller's phone into a structured pandas DataFrame indexed by datetime, with latitude and longitude columns.

One hypothesis was that Prof. Schueller’s weekend travel patterns changed over time, particularly when comparing 2015 (pre-pandemic), 2020, and 2023 (post-pandemic). The analysis revealed more frequent travel in 2015 and 2023 compared to 2020, likely reflecting pandemic restrictions.

<div id="carousel" class="carousel" style="position: relative; width: 100%; max-width: 800px; margin: auto;">
  <!-- Slide 1 -->
  <div class="slide active">
    <iframe src="figures/timelapse_2019.html" width="100%" height="600" frameborder="0"></iframe>
  </div>

  <!-- Slide 2 -->
  <div class="slide">
    <iframe src="figures/timelapse_2020.html" width="100%" height="600" frameborder="0"></iframe>
  </div>

  <!-- Slide 3 -->
  <div class="slide">
    <iframe src="figures/timelapse_2022.html" width="100%" height="600" frameborder="0"></iframe>
  </div>

  <!-- Navigation Buttons -->
  <button class="prev" onclick="changeSlide(-1)">&#10094;</button>
  <button class="next" onclick="changeSlide(1)">&#10095;</button>
</div>

<style>
  /* Carousel Styles */
  .carousel {
    overflow: hidden;
    position: relative; /* Ensure positioning for child elements */
  }

  .slide {
    display: none;
    text-align: center;
  }

  .slide.active {
    display: block;
  }

  .prev, .next {
    cursor: pointer;
    position: absolute;
    top: 50%; /* Center vertically */
    transform: translateY(-50%); /* Adjust for centering */
    width: auto;
    padding: 10px;
    font-size: 24px;
    color: white;
    background-color: rgba(0, 0, 0, 0.5);
    border: none;
    z-index: 10; /* Ensure buttons are above other elements */
    user-select: none; /* Prevent text selection on click */
  }

  .prev {
    left: 10px; /* Position on the left */
  }

  .next {
    right: 10px; /* Position on the right */
  }

  iframe {
    display: block;
    margin: auto;
    border: none;
  }
</style>

<script>
  let currentSlide = 0;

  function changeSlide(direction) {
    const slides = document.querySelectorAll('.slide');
    slides[currentSlide].classList.remove('active');
    currentSlide = (currentSlide + direction + slides.length) % slides.length;
    slides[currentSlide].classList.add('active');
  }

  // Initialize the first slide
  document.querySelector('.slide').classList.add('active');
</script>


The timelapse heatmaps support the hypothesis that Prof. Schueller’s travel patterns were more localized during 2020, reflecting the impact of the pandemic.

Find the full project 
<a href="https://colab.research.google.com/drive/16VBqXlgDpoVissV-YfJqjQtlUCJL9_00?usp=sharing" target="_blank">here</a>


## Skills and Technologies
#### Programming Languages:
Python
Java
C++

#### Porgrams and Technologies:
Google Collab
Blender
R-Studio
Canva

## Approach to Projects
Interactive Development
I utilize Google Colab for iterative and interactive data analysis, ensuring clear documentation and visualization throughout the process.

Best Practices
Drawing from the Python Data Science Handbook, I follow structured workflows for data wrangling, analysis, and visualization. This includes:
- Organizing code and comments for readability.
- Using modular functions to promote reusability and scalability.
- Incorporating rigorous testing to validate outputs.
  
Libraries I’ve used include Pandas, NumPy, Matplotlib, Plotly, and Mapbox for map visualizations.

## Fact-Based Insights
One of the key insights I’ve gained from my projects is the importance of inclusive and representative data, a concept emphasized in Factfulness by Hans Rosling. Selection bias can lead to misleading conclusions when datasets fail to reflect population diversity. This experience has reinforced my commitment to thinking critically, identifying gaps in data, and seeking diverse sources to ensure fairness and equity in analysis and outcomes. Inspired by Rosling's call to avoid one-size-fits-all narratives, I strive to uncover meaningful insights that serve broader, more inclusive audiences.


## Data Sources and Project Ideas
Response: Val and I were looking at the Consumer Price Index data (https://www.bls.gov/cpi/).
One idea was to work with the time-series data of prices over different presidential
administrations in the US. [2009-2017 (Obama); 2017-2021 (Trump); 2021-2024(Biden)]
We could also see if the consumer price index of good baskets in the US has changed not in
line with other countries' price indexes.
Data sources:

<a href="https://data.ecb.europa.eu/data/data-categories/prices-macroeconomic-and-sectoral-statistics/measuring-inflation-harmonised-index-consumer-prices-hicp/harmonised-index-consumer-prices-hicp/goods" target="_blank">Europen Central Bank</a>

<a href="https://data.imf.org/?sk=4ffb52b2-3653-409a-b471-d47b46d904b5&sid=1485878802128" target="_blank">International  Monetary Fund</a>

<a href="https://tradingeconomics.com/united-states/interest-rate" target="_blank">Trading Economics</a>

<a href="https://fred.stlouisfed.org/series/FEDFUNDS" target="_blank">FRED</a>

<a href="https://data.worldbank.org/indicator/FP.CPI.TOTL.ZG" target="_blank">World Bank Group</a>



