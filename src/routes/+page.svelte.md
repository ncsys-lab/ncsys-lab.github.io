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
   - Lee, C. Y., Achour, S., & Kapetanovic, Z. (2025).  _Low-power neuromorphic learning for micro-robotic controls in the wild_  (Under review).
   - Wang, Y. N., & Achour, S. (2024). Shem: A Hardware-Aware Optimization Framework for Analog Computing Systems. _arXiv preprint arXiv:2411.03557_ (Under review).
   - Yi, P., Yang, Y., Lee, C. Y., & Achour, S. (2025, March). Early Termination for Hyperdimensional Computing Using Inferential Statistics. In _Proceedings of the 30th ACM International Conference on Architectural Support for Programming Languages and Operating Systems, Volume 1_ (pp. 342-360).
   - Iyer, D., & Achour, S. (2025, March). Efficient Optimization with Encoded Ising Models. In _2025 IEEE International Symposium on High Performance Computer Architecture (HPCA)_ (pp. 85-98). IEEE.
   - Achour, S. (2025, January). Towards Design Optimization of Analog Compute Systems. In _Proceedings of the 30th Asia and South Pacific Design Automation Conference_ (pp. 857-864).
   - Lee, C. Y., Yi, P. (L.), Fite, M., Rao, T., Achour, S., & Kapetanovic, Z. (2025).  _HyperCam: Low-power onboard computer vision for IoT cameras_. In  _Proceedings of the 31st Annual International Conference on Mobile Computing and Networking (MobiCom)_. ACM, Hong Kong.
   - Chen, W. C., Wong, H. S. P., & Achour, S. (2024, June). Bitwise Adaptive Early Termination in Hyperdimensional Computing Inference. In _Proceedings of the 61st ACM/IEEE Design Automation Conference_ (pp. 1-6).
   - Sharma, R., & Achour, S. (2024). Compilation of Qubit Circuits to Optimized Qutrit Circuits. _Proceedings of the ACM on Programming Languages_, _8_(PLDI), 272-295.
   - Salcedo, W., McBeth, C., & Achour, S. (2024). Leveraging Generative AI for Rapid Design and Verification of a Vector Processor SoC. _IEEE Design & Test_.
   - Wang, Y. N., Cowan, G., Rührmair, U., & Achour, S. (2024, April). Design of Novel Analog Compute Paradigms with Ark. In _Proceedings of the 29th ACM International Conference on Architectural Support for Programming Languages and Operating Systems, Volume 2_ (pp. 269-286).

## Tools

## Fun Activities

## Attributions

This website is based on versions of CS110 and CS111's website created by
[John Ousterhout](https://web.stanford.edu/~ouster/cgi-bin/home.php) and
[Jerry Cain](https://profiles.stanford.edu/gerald-cain?tab=teaching) – thank you!
