---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

{% include hero.html %}

<main id="main">
  <!-- ======= About Section ======= -->
  <section id="about" class="about">
    <div class="container">

      <div class="section-title mt-3">
        <h2>About Us</h2>
        <strong>Trust is the core of our business.</strong>
      </div>

      <div class="row">
        <div class="col-lg-6">
          <img src="assets/img/about.jpg" class="img-fluid" alt="">
        </div>
        <div class="col-lg-6 pt-4 pt-lg-0">
          <p>
            We, ChunChun Sweets, started in the years 2000, are one of the foremost wholesale traders and suppliers of a wide variety of cashew kernels. Our offered range consists of best-grade Cashew Nuts.
          </p>
          <p>
            The main goal of our company is to constantly provide world-class cashew kernels to meet the changing customer’s needs. We have a vast amount of experience to procure the best quality cashew kernels.
          </p>
          <p>
            We value our partnerships. Trust is the core of our business. Our reasonable pricing, quality assured cashew kernels range and transparencies in deals are the main factors behind our success.
          </p>
          <p>
            We have an incredible reputation in domestic markets. We offer the entire range of products at affordable prices. The logistical support team in our company delivers all orders without any inconvenience.
          </p>
        </div>
      </div>

    </div>
  </section><!-- End About Section -->

  <!-- ======= Portfolio Section ======= -->
  <section id="portfolio" class="portfolio">
    <div class="container">

      <div class="section-title">
        <h2>Products Range</h2>
      </div>

      <div class="row portfolio-container">

        {% for product in site.home_page_products %}

          <div class="col-lg-4 col-md-6 portfolio-item filter-app wow fadeInUp">
            <div class="portfolio-wrap">
              <figure>
                <img src="assets/img/products/{{ product.image }}" class="img-fluid" alt="">
                <a href="assets/img/products/{{ product.image }}" data-gallery="portfolioGallery" class="link-preview portfolio-lightbox" title="Preview"><i class="bx bx-plus"></i></a>
                <a href="portfolio-details.html" class="link-details" title="More Details"><i class="bx bx-link"></i></a>
              </figure>

              <div class="portfolio-info">
                <h4><a href="portfolio-details.html">{{ product.name }}</a></h4>
                <p>{{ product.name }}</p>
              </div>
            </div>
          </div>
        {% endfor %}
      </div>

    </div>
  </section><!-- End Portfolio Section -->
</main>

{% include contact.html %}
