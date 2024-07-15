---
title: "Good practices"
teaching: 0
exercises: 0
questions:
- "How can we make the best use of the resources at the Analysis Facility"
objectives:
- "To always consider the _good practices_, specially when working remotely"
keypoints:
- "Make a good use of the resources at the analysis facility is important to keep it working properly"

---

Resource Limitations on a running a job:
and HTCondor may configure the system to prevent using all the resources on a machine.

Jobs may see
>
> - A private (non-shared) /tmp and /var/tmp directory
>
> - A private (non-shared) /dev/shm
>
> - A limit on the amount of memory they can allocate, above which the job may be placed on hold or evicted by the system.
>
> - A limit on the amount of CPU cores the may use, above which the job may be blocked, and will run very slowly
>
{: .callout}

JupyterLab

> Since applications are time limited, please remember to request only the resources that you need.
{: .callout}

Acceptable Use policy




{% include links.md %}

