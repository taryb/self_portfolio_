<script>
import feather from 'feather-icons';
import ContactDetails from '@/components/contact/ContactDetails.vue';

export default {
	components: {
		ContactDetails,
	},
	data: () => {
		return {
			contacts: [
				{
					id: 1,
					name: 'Fairfield, CA',
					icon: 'map-pin',
				},
				{
					id: 2,
					name: 'tarybounavong@gmail.com',
					icon: 'mail',
				},
			],
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div
		class="container mx-auto flex flex-col-reverse md:flex-row py-5 md:py-10 md:mt-10"
	>

		<!-- Contact details -->
		<ContactDetails :contacts="contacts" />
	</div>
</template>
