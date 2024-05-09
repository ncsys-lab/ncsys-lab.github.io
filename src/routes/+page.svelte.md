---
title: 'NCS Lab'
---

<script lang="ts">
  import { base } from '$app/paths';
  import Calendar from '$lib/Calendar.svelte';
  import { class_data, fixupLink } from '$lib/classData';

  import Instructor from '$lib/Instructor.svelte';
  import Callout from '$lib/Callout.svelte';
</script>

# Stanford Novel Computing Systems Lab

## Lab Description

We are interested in developing novel computing systems for unconventional computing paradigms and emerging hardware platforms.

## People

<!-- **Staff Mailing List:** -->
<!-- [cs45-spr2223-staff@lists.stanford.edu](mailto:cs45-spr2223-staff@lists.stanford.edu) -->

<div style="display: flex; flex-wrap: wrap;">
	{#each class_data.instructors as instructor}
		<Instructor
			src={fixupLink(instructor.image)}
			name={instructor.name}
			role={instructor.role}
			email={instructor.email}
			direction={instructor.direction}
			website={instructor.website}
			officeHours={instructor.officeHours}
		/>
	{/each}
</div>

## News

## Publications

## Tools

## Fun Activities

## Attributions

This website is based on versions of CS110 and CS111's website created by
[John Ousterhout](https://web.stanford.edu/~ouster/cgi-bin/home.php) and
[Jerry Cain](https://profiles.stanford.edu/gerald-cain?tab=teaching) – thank you!
