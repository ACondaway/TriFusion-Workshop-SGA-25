---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an
# online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "SIGGRAPH Asia 2025"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: "TBD (Conference Venue)"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "cn"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the workshop
latitude: "35.6762"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "139.6503"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "Dec 8, 2025"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "9:00 am - 5:00 pm JST"    # human-readable times for the workshop e.g., "9:00 am - 4:30 pm CEST (7:00 am - 2:30 pm UTC)"
startdate: 2025-12-08      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2025-12-08        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
organizers: ["Ping Luo (HKU)", "Xiaokang Yang (SJTU)", "Yao Mu (SJTU)", "Yichao Yan (SJTU)", "Ailing Zeng (Anuttacon)", "Jingbo Wang (Shanghai AI Lab)"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
student_leaders: ["Liang Xu (SJTU/EIT)", "Congsheng Xu (SJTU)", "Tengjie Zhu (SJTU)", "Kaixuan Wang (HKU)"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["acondaway@sjtu.edu.cn"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes: "https://pad.carpentries.org/trifusion-siggraph-asia-2025"  # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
eventbrite:           # optional: alphanumeric key for Eventbrite registration, e.g., "1234567890AB" (if Eventbrite is being used)

---

{% comment %} See instructions in the comments below for how to edit specific sections of this workshop template. {% endcomment %}

{% comment %}
HEADER

Edit the values in the block above to be appropriate for your workshop.
If the value is not 'true', 'false', 'null', or a number, please use
double quotation marks around the value, unless specified otherwise.
And run 'make workshop-check' *before* committing to make sure that changes are good.
{% endcomment %}





{% comment %}
Check DC curriculum
{% endcomment %}

{% if site.carpentry == "dc" %}
{% unless site.curriculum == "dc-astronomy" or site.curriculum == "dc-ecology" or site.curriculum == "dc-genomics" or site.curriculum == "dc-geospatial" or site.curriculum == "dc-image" or site.curriculum == "dc-socsci" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Data Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>dc-image</code>, <code>dc-astronomy</code>, <code>dc-ecology</code>, <code>dc-genomics</code>, <code>dc-socsci</code>, or <code>dc-geospatial</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}

{% comment %}
Check SWC curriculum
{% endcomment %}

{% if site.carpentry == "swc" %}
{% unless site.curriculum == "swc-inflammation" or site.curriculum == "swc-gapminder" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Software Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>swc-inflammation</code>, or <code>swc-gapminder</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}

{% comment %}
EVENTBRITE

This block includes the Eventbrite registration widget if
'eventbrite' has been set in the header.  You can delete it if you
are not using Eventbrite, or leave it in, since it will not be
displayed if the 'eventbrite' field in the header is not set.
{% endcomment %}
{% if page.eventbrite %}
<strong>Some adblockers block the registration window. If you do not see the
  registration box below, please check your adblocker settings.</strong>
<div id="eventbrite-widget-container"></div>
<script src="https://www.eventbrite.com/static/widgets/eb_widgets.js"></script>
<script type="text/javascript">
    window.EBWidgets.createWidget({
        // Required
        widgetType: 'checkout',
        eventId: {{page.eventbrite}},
        iframeContainerId: 'eventbrite-widget-container',
    });
</script>
{% endif %}


<div class="workshop-header">
  <h1>TriFusion Workshop@SIGGRAPH Asia 2025</h1>
  <div class="subtitle">
    Towards Embodied Intelligence Across 
    <span class="domain-emoji human">Humans 😐</span>, 
    <span class="domain-emoji avatar">Avatars 🫥</span>, and 
    <span class="domain-emoji robot">Humanoid Robotics 🤖</span>
  </div>
</div>

<h2 id="about">About the Workshop</h2>

<div class="row">
  <div class="col-md-8">
    <p>
      TriFusion: Towards Embodied Intelligence Across Humans, Avatars, and Humanoid Robotics aims to catalyze interdisciplinary dialogue and innovation at the intersection of computer graphics, artificial intelligence, robotics, and cognitive science. As digital avatars and humanoid robots increasingly act as proxies and collaborators in both virtual and physical environments, bridging the simulation-to-reality (sim-to-real) gap becomes a critical challenge for achieving believable, reliable, and adaptive embodied behaviors. This workshop investigates the shared principles and enabling technologies that support the seamless transfer of perception, cognition, and motor skills across human users, digital surrogates, and robotic agents.   
    </p>
    
    <p>
      Key topics include sensorimotor learning across simulated and real embodiments, physically based and data-driven motion synthesis, neural and biomechanical modeling for animation and control, real-time avatar retargeting, cross-domain telepresence, and the integration of digital twins as testbeds for embodied cognition. By uniting researchers and practitioners from graphics, animation, and robotics, TriFusion seeks to establish foundational frameworks for unified embodiment, advance collaborative simulation platforms, and chart a research agenda that supports scalable, adaptive, and human-aligned intelligence across both real and synthetic agents.
    </p>
    
    
    <h3>Key Research Areas</h3>
    <div class="row research-focus">
      <div class="col-md-6">
        <ul>
          <li>Embodied Intelligence</li>
          <li>Human-Avatar Interaction</li>
          <li>Humanoid Robotics</li>
        </ul>
      </div>
      <div class="col-md-6">
        <ul>
          <li>Cross-Domain Transfer Learning</li>
          <li>Multi-Modal Perception</li>
          <li>Cognitive Skill Transfer</li>
  </ul>
      </div>
    </div>
  </div>
  
  <div class="col-md-4">
    <div class="panel panel-primary">
      <div class="panel-heading">
        <h3 class="panel-title">Workshop Details</h3>
      </div>
      <div class="panel-body">
        <p><strong>Date:</strong> {{page.humandate}}</p>
        <p><strong>Time:</strong> {{page.humantime}}</p>
        <p><strong>Venue:</strong> {{page.venue}}</p>
        <p><strong>Location:</strong> {{page.address}}</p>
        <p><strong>Contact:</strong> 
  {% for email in page.email %}
            <a href="mailto:{{email}}">{{email}}</a>
  {% endfor %}
        </p>
      </div>
    </div>
  </div>
</div>

<h2 id="schedule">Schedule & Activities</h2>

<div class="row">
  <div class="col-md-12">
<p class="text-center">
      <em>A comprehensive full-day exploration of embodied intelligence across humans, avatars, and humanoid robotics</em>
    </p>
  </div>
</div>

{% include trifusion-schedule.html %}

<hr/>

<h2 id="people">Speakers & Organizers</h2>

<h3>Keynote Speakers</h3>
<div class="row">
  <div class="col-md-4">
    <div class="panel panel-info speaker-panel">
      <div class="panel-heading">
        <h4>Jingyi Yu</h4>
        <small>ShanghaiTech University</small>
      </div>
      <div class="panel-body">
        <p>Expert in computer vision, computational photography, and virtual/augmented reality technologies.</p>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="panel panel-info speaker-panel">
      <div class="panel-heading">
        <h4>Ziwei Liu</h4>
        <small>Nanyang Technological University</small>
      </div>
      <div class="panel-body">
        <p>Leading researcher in computer vision, human-centric AI, and advanced avatar technologies.</p>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="panel panel-info speaker-panel">
      <div class="panel-heading">
        <h4>Jiajun Wu</h4>
        <small>Stanford University</small>
      </div>
      <div class="panel-body">
        <p>Pioneer in embodied AI and robotics, focusing on intelligent agents and embodied learning.</p>
      </div>
    </div>
  </div>
</div>

<h3>Organizers</h3>
<div class="row organizer-section">
  <div class="col-md-6">
    <h4>Senior Organizers</h4>
    <ul class="list-unstyled">
      <li><strong>Ping Luo</strong> - The University of Hong Kong</li>
      <li><strong>Xiaokang Yang</strong> - Shanghai Jiao Tong University</li>
      <li><strong>Yao Mu</strong> - Shanghai Jiao Tong University</li>
      <li><strong>Yichao Yan</strong> - Shanghai Jiao Tong University</li>
      <li><strong>Ailing Zeng</strong> - Anuttacon</li>
      <li><strong>Jingbo Wang</strong> - Shanghai AI Lab</li>
    </ul>
  </div>
  
  <div class="col-md-6">
    <h4>Student Leaders</h4>
    <ul class="list-unstyled">
      <li><strong>Liang Xu</strong> - SJTU/EIT</li>
      <li><strong>Congsheng Xu</strong> - Shanghai Jiao Tong University</li>
      <li><strong>Tengjie Zhu</strong> - Shanghai Jiao Tong University</li>
      <li><strong>Kaixuan Wang</strong> - The University of Hong Kong</li>
    </ul>
    
    <h4>Program Committee</h4>
    <p><small>
      Yitian Liu (SJTU), Yuzhang Li (TJU), Yibin Liu (NEU), 
      Yuhao Zhang (SJTU), Wanxi Dong (SUSTech)
    </small></p>
  </div>
</div>

<div class="row">
  <div class="col-md-12">
    <div class="panel panel-default">
      <div class="panel-body text-center">
        <h4>Join Our Community</h4>
        <p>Connect with researchers, practitioners, and enthusiasts working on embodied intelligence.</p>
        <p>
          <strong>Contact:</strong> 
          {% for email in page.email %}
            <a href="mailto:{{email}}" class="btn btn-primary">{{email}}</a>
          {% endfor %}
        </p>
      </div>
    </div>
  </div>
</div>
