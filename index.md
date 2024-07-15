---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an
# online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "2024 US ATLAS Workshop @ University of Washington, Seattle"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
#address: "FIXME"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
#country: "FIXME"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
#language: "FIXME"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the workshop
#latitude: "45"        # decimal latitude of workshop venue (use https://www.latlong.net/)
#longitude: "-1"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "July 17, 2024"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
#humantime: "FIXME"    # human-readable times for the workshop e.g., "9:00 am - 4:30 pm CEST (7:00 am - 2:30 pm UTC)"
#startdate: FIXME      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
#enddate: FIXME        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Verena Martinez", "Yuan-Tang Chou", "Cristiano Alpigiani"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
#helper: ["helper one", "helper two"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
#email: ["first@example.org","second@example.org"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes: https://usatlas.readthedocs.io/projects/af-docs/en/latest/ # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
#eventbrite:           # optional: alphanumeric key for Eventbrite registration, e.g., "1234567890AB" (if Eventbrite is being used)
---

<div class="alert alert-success">
  This tutorial wants to guide the users through the baseline setup to submit a job at an analysis facility (UChicago in this tutorial). It is based on the material presented in this <a href="https://cecilia-duran.github.io/2022-04_gh_usatlas_af_qst/index.html">Quickstart</a> tutorial (credits Cecilia Duran).
</div>

> ## Prerequisites
>
>
> This assumes you already have:
>
> - <strong>A CERN account</strong>
>
> - <strong>The respective X509 Proxy Certificate, e.g. to access ATLAS Data</strong>. You can use the same you copied on lxplus (in case you already did it) or download it from this CERN page: <a href="https://cafiles.cern.ch/cafiles/">https://cafiles.cern.ch/cafiles/</a>.
>
>
{: .prereq}


<h2 id="general">General Information</h2>

<hr/>

{% comment %} INTRODUCTION {% endcomment %}

{% include swc/intro.html %}

<p><br /></p>
<div class="text-center">
  <a href="https://indico.cern.ch/event/1348862/" target="_blank" rel="noopener noreferrer">
    <button type="button" class="btn btn-info" style="font-size:large;text-align:center">US ATLAS Summer Workshop 2024</button>
  </a>
</div>
<p><br /></p>

{% comment %} AUDIENCE {% endcomment %}

{% include swc/who.html %}

{% comment %} LOCATION {% endcomment %}

<p id="where">
  <strong>Where:</strong>
  <strong>C211 (PAC)</strong>. More info <a href="">here</a>.
</p>

{% comment %} DATE {% endcomment %}

{% if page.humandate %}
<p id="when">
  <strong>When:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% comment %} SPECIAL REQUIREMENTS {% endcomment %}

<p id="requirements">
  <strong>Requirements:</strong>
    No specific requirements. Participants must bring a laptop with a Mac, Linux, or Windows operating system.
</p>

{% comment %} CONTACT EMAIL ADDRESS {% endcomment %}

<p id="contact">
  <strong>Contact:</strong>
  Please email <a href='mailto:Verena.Martinez@cern.ch,yuan-tang.chou@cern.ch,Cristiano.Alpigiani@cern.ch'>the tutorial organizers</a>. 

  
</p>

{% comment%} CODE OF CONDUCT {% endcomment %}

<h2 id="code-of-conduct">Code of Conduct</h2>

<hr/>

<p> Everyone who participates in Carpentries activities is required to conform to the <a href="https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html">Code of Conduct</a>. 
This document also outlines how to report an incident if needed. </p>

{% comment %} DOCUMENTATION {% endcomment %}

<h2 id="Documentation">Documentation</h2>

<hr/>

<p> You can find a lot of useful information in <a href="https://usatlas.readthedocs.io/projects/af-docs/en/latest/">Public Documentation for US ATLAS Analysis Facilities</a>. </p>

<p>You can find the list of ATLAS software tutorials here <a href="https://twiki.cern.ch/twiki/bin/viewauth/AtlasComputing/SoftwareTutorial">SoftwareTutorial</a>, while here <a href="https://atlassoftwaredocs.web.cern.ch/ASWTutorial/TutorialWeek/asking_questions/">Where to ask questions</a> you can find the main mailing lists to get assistance on software.</p>

  
{% comment%} SCHEDULE {% endcomment %}

{% include base_path.html %}

<h2 id="schedule">Schedule</h2>

<hr/>

<div class="syllabus">
  
  <table class="table table-striped">
    <tr> <td colspan="3"> <font color="Bright Gold"><strong>Account setup</strong></font> </td> </tr>
     <tr> <td class="col-md-2">15:00</td>      <td class="col-md-3"><a href="{{ relative_root_path }}/00-uchicago_af_intro/index.html">Introduction to Analysis Facilities</a> </td> <td class="col-md-7"> Why would you want to work on US-ATLAS Analysis Facilities? </td> </tr>      
     <tr> <td class="col-md-2">15:10</td> <td class="col-md-3"><a href="{{ relative_root_path }}/01-accountrequest/index.html">UChicago account request</a> </td> <td class="col-md-7"> How can I join the UChicago US-ATLAS analysis facility? </td> </tr>
     <tr> <td class="col-md-2">15:20</td>       <td class="col-md-3"><a href="{{ relative_root_path }}/02-atlasenv/index.html">ATLAS environment setup</a> </td> <td class="col-md-7"> How does this differ from using lxplus? </td> </tr>
    <tr> <td colspan="3"> <font color="LimeGreen"><strong>Overview of the main</strong></font> </td> </tr>
     <tr> <td class="col-md-2">15:30</td>       <td class="col-md-3"><a href="{{ relative_root_path }}/03-htcondor/index.html">HT Condor</a> </td> <td class="col-md-7"> How do I submit jobs with HTCondor? </td> </tr>
     <tr> <td class="col-md-2">15:30</td>       <td class="col-md-3"><a href="{{ relative_root_path }}/04-jupyter_lab/index.html">Jupyter Lab</a> </td> <td class="col-md-7"> What is JupyterLab and how will it help the analysis process? </td> </tr>
     <tr> <td class="col-md-2">15:30</td>       <td class="col-md-3"><a href="{{ relative_root_path }}/05-coffea_casa/index.html">Coffea Casa </a> </td> <td class="col-md-7"> What is Coffea Casa? </td> </tr>
     <tr> <td colspan="3"> <font color="LimeGreen"><strong>Extra</strong></font> </td> </tr>
     <tr> <td class="col-md-2">EXTRA</td>       <td class="col-md-3"><a href="{{ relative_root_path }}/06-goodpractices/index.html">Good Practices</a> </td> <td class="col-md-7"> How can we make the best use of the resources at US-ATLAS Analysis Facilities? </td> </tr>
    <tr> <td colspan="3"> <a href="https://indico.cern.ch/event/1258537/surveys/4591?token=ea7c57a7-bea5-402d-9358-8250f04a7dc4" target="_blank" rel="noopener noreferrer">POST-Tutorial Survey</a> </td> </tr>
  </table>

</div>

<!---
{% comment %} SURVEYS {% endcomment %}

<h2 id="surveys">Surveys</h2>

<hr/>

<p>Please be sure to complete these surveys before and after the workshop.</p>
<p><a href="https://indico.cern.ch/event/1258537/surveys/4590?token=17f96380-c23b-4666-bdcc-3390d74fbd52">Pre-workshop Survey</a></p>
<p><a href="">Post-workshop Survey</a> Do we want to have one??????</p>

-->
