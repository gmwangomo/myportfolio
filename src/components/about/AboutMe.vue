<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'HI, I am Gwakisa Mwangomo!',
				},
				{
					id: 2,
					bio:
						'Fullstack Developer at GalemTech.',
				},
				{
					id: 3,
					bio:
						"Also the betters developer and with high explessing in the coding and development of project",
				}
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/hor-pf.jpg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
