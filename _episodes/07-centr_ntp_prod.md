---
title: "Centralised ntuple production system"
teaching: 5
exercises: 0
questions:
- "How can I easily submit and manage a ntuple production?"
objectives:
- " Produce ntuples "

keypoints:
- "This will user ntuple production step very easy"

---

- Built a system to centrally produce user/CP ntuples as we do already for MCProd, group production, etc using ProdSys

- Main advantages: ProdSys is a well known and robust system, and allows to “follow” the standard workflow (e.g. ntuple production linked directly to the parent DAOD production)

- Analysers with group production roles create the gTag, the request, submit and manage the production (retry the jobs and change only some job parameters, #GB/jobs))

![image info](./../fig/Screenshots-NtupleProduction.png){:width="1000"}{: .image-with-shadow }

A detailed guide on how to submit a production can be found here

<p><br /></p>
<div class="text-center">
  <a href="https://atlassoftwaredocs.web.cern.ch/guides/ntuples_production/" target="_blank" rel="noopener noreferrer">
    <button type="button" class="btn btn-info" style="font-size:large;text-align:center">Centralised N-tuple Production</button>
  </a>
</div>
<p><br /></p>


<!----------------------------------- fin --------------------------------------------->
{% include links.md %}

