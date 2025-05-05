<template>
  <div 
    :class="[
      'transform transition-all duration-200 border-black border-3',
      bgColorClass,
      shadowClass,
      hoverClass,
      roundedClass
    ]"
  >
    <slot></slot>
  </div>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps({
  bgColor: {
    type: String,
    default: 'white'
  },
  shadow: {
    type: String,
    default: 'md',
    validator: (value) => ['none', 'sm', 'md', 'lg'].includes(value)
  },
  hover: {
    type: Boolean,
    default: false
  },
  rounded: {
    type: String,
    default: 'md',
    validator: (value) => ['none', 'sm', 'md', 'lg', 'xl'].includes(value)
  }
});

const bgColorClass = computed(() => {
  const colors = {
    'white': 'bg-white',
    'primary': 'bg-primary-500 text-white',
    'secondary': 'bg-secondary-500 text-white',
    'yellow': 'bg-[var(--color-accent-yellow)]',
    'orange': 'bg-[var(--color-accent-orange)] text-white',
    'pink': 'bg-[var(--color-accent-pink)] text-white',
    'red': 'bg-[var(--color-accent-red)] text-white',
    'gray': 'bg-gray-100'
  };
  
  return colors[props.bgColor] || 'bg-white';
});

const shadowClass = computed(() => {
  const shadows = {
    'none': '',
    'sm': 'shadow-neo-sm',
    'md': 'shadow-neo',
    'lg': 'shadow-neo-lg'
  };
  
  return shadows[props.shadow] || 'shadow-neo';
});

const hoverClass = computed(() => {
  return props.hover ? 'hover:-translate-y-1 hover:translate-x-1' : '';
});

const roundedClass = computed(() => {
  const roundedSizes = {
    'none': 'rounded-none',
    'sm': 'rounded-sm',
    'md': 'rounded',
    'lg': 'rounded-lg',
    'xl': 'rounded-xl'
  };
  
  return roundedSizes[props.rounded] || 'rounded';
});
</script>

<style>
.border-3 {
  border-width: 3px;
}

.shadow-neo {
  box-shadow: var(--shadow-neo);
}

.shadow-neo-sm {
  box-shadow: var(--shadow-neo-sm);
}

.shadow-neo-lg {
  box-shadow: var(--shadow-neo-lg);
}
</style> 