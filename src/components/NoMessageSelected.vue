<!--
  - @copyright 2019 Christoph Wurst <christoph@winzerhof-wurst.at>
  -
  - @author 2019 Christoph Wurst <christoph@winzerhof-wurst.at>
  -
  - @license AGPL-3.0-or-later
  -
  - This program is free software: you can redistribute it and/or modify
  - it under the terms of the GNU Affero General Public License as
  - published by the Free Software Foundation, either version 3 of the
  - License, or (at your option) any later version.
  -
  - This program is distributed in the hope that it will be useful,
  - but WITHOUT ANY WARRANTY; without even the implied warranty of
  - MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  - GNU Affero General Public License for more details.
  -
  - You should have received a copy of the GNU Affero General Public License
  - along with this program.  If not, see <http://www.gnu.org/licenses/>.
  -->

<template>
	<AppContentDetails>
		<div id="emptycontent">
			<IconMail :size="65" />
			<h2>{{ t('mail', 'No message selected') }}</h2>
			<p />
		</div>
	</AppContentDetails>
</template>

<script>
import { NcAppContentDetails as AppContentDetails } from '@nextcloud/vue'
import IconMail from 'vue-material-design-icons/Email'

export default {
	name: 'NoMessageSelected',
	components: {
		AppContentDetails,
		IconMail,
	},
}
</script>

<style scoped>
h2,
p {
	text-align: center;
}
</style>
