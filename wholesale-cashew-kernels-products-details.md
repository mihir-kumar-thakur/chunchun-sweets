---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Wholesale Cashew Kernels | Products from ChunChun Sweets
layout: default
---


<main id="main">
  <!-- ======= Breadcrumbs ======= -->
  <div class="breadcrumbs">
    <div class="container">
      <div class="d-flex justify-content-between align-items-center">
        <h2>List of Cashew Kernels</h2>
        <ol>
          <li><a href="/">Home</a></li>
          <li>Cashew Kernels</li>
        </ol>
      </div>
      <hr />
    </div>
  </div>
  <!-- End Breadcrumbs -->
  <div class="inner-page">
    <div class="container">
      <div class="row">
        {% for product in site.products %}
          <div class="col-md-4 mb-3">
            <div class="card h-100">
              <div class="d-flex justify-content-between position-absolute w-100">
                <div class="label-new">
                  <span class="text-white bg-success small d-flex align-items-center px-2 py-1">
                  <i class="fa fa-star" aria-hidden="true"></i>
                  <span class="ml-1">Fresh</span>
                  </span>
                </div>
                <div class="label-sale">
                  <span class="text-white bg-primary small d-flex align-items-center px-2 py-1">
                  <i class="fa fa-tag" aria-hidden="true"></i>
                  <span class="ml-1">Best Quality</span>
                  </span>
                </div>
              </div>
              <a href="#">
              <img src="assets/img/products/{{ product.image }}" class="card-img-top" alt="Product">
              </a>
              <div class="card-body px-2 pb-2 pt-1">
                <div class="d-flex justify-content-between">
<!--                   <div>
                    <p class="h4 text-primary">$129,99</p>
                  </div> -->
<!--                   <div>
                    <a href="#" class="text-secondary lead" data-toggle="tooltip" data-placement="left" title="Compare">
                    <i class="fa fa-line-chart" aria-hidden="true"></i>
                    </a>
                  </div> -->
                </div>
                                <p class="mb-0">
                  <strong>
                  <a href="#" class="text-secondary">{{ product.name }}</a>
                  </strong>
                </p>
                <p class="text-warning d-flex align-items-center mb-2">
                  <i class="fa fa-star" aria-hidden="true"></i>
                  <i class="fa fa-star" aria-hidden="true"></i>
                  <i class="fa fa-star" aria-hidden="true"></i>
                  <i class="fa fa-star" aria-hidden="true"></i>
                  <i class="fa fa-star" aria-hidden="true"></i>
                </p>
                <div class="d-flex mb-3 justify-content-between">
                  <div>
                    <p class="mb-0 small"><b>Packing Type: </b> {{ product.packing_type }}</p>
                    <p class="mb-0 small"><b>Packaging Size: </b> 10Kg</p>
                    <p class="mb-0 small"><b>Processing Type: </b> {{ product.processing_type }}</p>
                  </div>
                  <div class="text-right">
                    <p class="mb-0 small"><b>All India Transportation</b></p>
                    <p class="mb-0 small"><b>Color: </b> White</p>
                    <p class="mb-0 small"><b>Life: </b> 6 Months</p>
                  </div>
                </div>
                <div class="d-flex justify-content-between">
                  <div class="col px-0">
                    <a href='https://wa.me/+919224102279' target='_blank' class="btn btn-success  btn-block">
                      WhatsApp
                      <i class= "fa fa-whatsapp"></i>
                    </a>
                    <a href="tel:+91 92241 02279" target="_blank" class="btn btn-outline-primary btn-block">
                      <i class="fa fa-mobile" aria-hidden="true"></i>
                      +91 92241 02279
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        {% endfor %}
      </div>
    </div>
    <div class="container">
      <hr />
    </div>
  </div>
</main>
<!-- End #main -->
