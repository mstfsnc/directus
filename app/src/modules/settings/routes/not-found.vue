<template>
	<private-view :title="$t('page_not_found')">
		<template #navigation>
			<settings-navigation />
		</template>

		<div class="not-found">
			<v-info :title="$t('page_not_found')" icon="not_interested">
				{{ $t('page_not_found_body') }}
			</v-info>
		</div>
	</private-view>
</template>

<script lang="ts">
import { defineComponent } from '@vue/composition-api';
import SettingsNavigation from '../components/navigation.vue';

export default defineComponent({
	components: { SettingsNavigation },
});
</script>

<style lang="scss" scoped>
.not-found {
	display: flex;
	align-items: center;
	justify-content: center;
	padding: 20vh 0;
}
</style>
