<template>
  <div class="text-center">
    <span class="rounded-full uppercase px-2 py-1 text-xs font-bold whitespace-no-wrap"
          :class="badgeExtraClasses"
          :style="{ backgroundColor: backgroundColor(), color: textColor() }"
    >{{ __(displayValue()) }}</span>
  </div>
</template>

<script>
import colors from '../mixins/colors';
import display from '../mixins/display';

export default {
  props: ['resourceName', 'field'],
  mixins: [colors, display]
}
</script>
