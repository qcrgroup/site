---
title: "Quantitative Criminology Research Cluster"
layout: splash
permalink: /pages/members/
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
  overlay_image: /assets/images/splash/London_gangs_1.png
  actions:
    - label: "Members"
      url: "/pages/members/"
    - label: "Our Research"
      url: "/pages/research/"
    - label: "Our Partners"
      url: "/pages/partners/"

partners_andrea:

  - image_path: /assets/images/splash/cambridge_logo.png
    alt: "University of Cambridge"
    url: "http://www.cam.ac.uk"
  - image_path: /assets/images/splash/deakin.png
    alt: "Deakin University"
    url: "https://partner3.com"
  - image_path: /assets/images/splash/merseyside_logo.png
    alt: "Merseyside Police"
    url: "https://partner3.com"
  - image_path: /assets/images/splash/met_logo.png
    alt: "MET Police"
    url: "https://partner3.com"
  - image_path: /assets/images/splash/taklinghate.png
    alt: "MET Police"
    url: "https://partner3.com"
  - image_path: /assets/images/splash/siena.png
    alt: "MET Police"
    url: "https://partner3.com"
  - image_path: /assets/images/splash/hilst.png
    alt: "MET Police"
    url: "https://partner3.com"
  - image_path: /assets/images/splash/modena.png
    alt: "MET Police"
    url: "https://partner3.com"
  - image_path: /assets/images/splash/eu.png
    alt: "EU"
    url: "https://partner3.com"



---



<div class="profile-container">
  <div class="profile-card">
    <div class="profile-header">
      <h2>Andrea Giovannetti, Ph.D</h2>
    </div>
    <div class="profile-content">
      <img src="{{ site.baseurl }}/assets/images/andrea_logo.jpg" alt="Andrea Logo" class="profile-image">
      <div class="profile-text">
        <blockquote>
          Reality is a set of interconnected entities, and the properties of such interconnections matter for the control of crucial phenomena such as the diffusion of behaviours. In my work, I develop analytical models and apply high-	  power computational and statistical techniques to investigate and predict the diffusion of behaviours on human and economic networks.
        </blockquote>
        <p class="research-interests"><b>Research Interests:</b> Networks, Statistical Analysis of Organized Crime, Simulations, Economics</p>
        <div class="button-container">
          <button id="expand-bio-button" class="button">Expand BIO</button>
          <a href="https://scholar.google.com.au/citations?user=HileARUAAAAJ&hl=it" class="button">Google Scholar</a>
          <a href="mailto:andrea.giovannetti@acu.edu.au" class="button">Email Contact</a>
        </div>
      </div>
    </div>
  </div>
</div>

<div id="full-bio" class="profile-full-bio">
  <h3>BIO</h3>
  <p>Andrea is Principal Investigator at the <a href="https://hilstlab.org/">HILSTLab</a>, and Assistant Professor in Economics at the <a href="https://www.acu.edu.au/about-acu/faculties-directorates-and-staff/faculty-of-law-and-business">Faculty of Law and Business</a> of the Australian Catholic University.</p>
  <p>Before joining ACU, Andrea was a <strong>Marie Skłodowska-Curie fellow</strong> at the <a href="https://www.crim.cam.ac.uk">Institute of Criminology</a> of the University of Cambridge, UK. The Marie Skłodowska-Curie fellowship is the most prestigious individual grant offered by the European Union and one of the most competitive grants in the world.</p>
  <p>He obtained his PhD in Economics in 2018 from the <a href="https://www.southampton.ac.uk/">University of Southampton</a>, UK. From 2018 to 2021 he worked as a research fellow at the <a href="https://www.uts.edu.au/about/uts-business-school/economics-department">Economics Department</a> of University of Technology Sydney.</p>
  <p>Andrea currently holds a position as associate researcher at <a href="https://www.darwin.cam.ac.uk/">Darwin College</a>, Cambridge and he is an active member of the <a href="https://www.vrc.crim.cam.ac.uk/">Violence Research Centre</a> of the Institute of Criminology of Cambridge. The institute frequently ranks as the top Criminology institution of the world. He has active, operative collaborations with the <strong>London Metropolitan Police Force</strong> (the largest police force of Europe), as well as <strong>Merseyside Police</strong> and <strong>Cambridgeshire Police force</strong>.</p>
  <h3>MAIN GRANTS (USD Equivalent)</h3>
  <ul>
    <li>Breaking networks of youth serious violence, ESRC, 2024 (team member) (<strong>147,070 USD</strong>)</li>
    <li>Marie Sklodowska-Curie Individual Fellowship (eval. top 1%), 2020 (<strong>256,950 USD</strong>)</li>
    <li>Best Lecturer of the University, University of Technology Sydney, 2020 (<strong>2,513 USD</strong>)</li>
    <li>Research Grant, University of Cambridge, 2019 (<strong>2,751 USD</strong>)</li>
    <li>Economic and Social Research Council, 2014 (<strong>73,000 USD</strong>)</li>
    <li>Venini Award for Best MSc Dissertation, 2013 (<strong>30,000 USD</strong>)</li>
  </ul>

<section class="partners">
  <h2>My Collaborations and Partners</h2>
  <div class="partners-container">
    {% for partner in page.partners_andrea %}
      <a href="{{ partner.url }}">
        <img src="{{ partner.image_path | relative_url }}" alt="{{ partner.alt }}">
      </a>
    {% endfor %}
  </div>
</section>


</div>

<script>
  document.addEventListener('DOMContentLoaded', function () {
    var expandButton = document.getElementById('expand-bio-button');
    var fullBio = document.getElementById('full-bio');

    expandButton.addEventListener('click', function (e) {
      e.preventDefault();
      if (fullBio.style.display === 'none' || fullBio.style.display === '') {
        fullBio.style.display = 'block';
        expandButton.textContent = 'Collapse BIO';
      } else {
        fullBio.style.display = 'none';
        expandButton.textContent = 'Expand BIO';
      }
    });
  });
</script>