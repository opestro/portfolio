<template>
  <button 
    :class="[
      'font-bold px-6 py-3 transition-all duration-200 transform border-black border-3 active:translate-x-1 active:translate-y-1 active:shadow-none',
      variantClasses,
      sizeClasses
    ]"
    :disabled="disabled"
  >
    <slot></slot>
  </button>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps({
  variant: {
    type: String,
    default: 'primary',
    validator: (value) => ['primary', 'secondary', 'yellow', 'orange', 'pink', 'red', 'white'].includes(value)
  },
  size: {
    type: String,
    default: 'md',
    validator: (value) => ['sm', 'md', 'lg'].includes(value)
  },
  disabled: {
    type: Boolean,
    default: false
  }
});

const variantClasses = computed(() => {
  const variants = {
    'primary': 'bg-primary-500 text-white shadow-neo hover:bg-primary-600',
    'secondary': 'bg-secondary-500 text-white shadow-neo hover:bg-secondary-600',
    'yellow': 'bg-[var(--color-accent-yellow)] text-black shadow-neo hover:bg-yellow-300',
    'orange': 'bg-[var(--color-accent-orange)] text-white shadow-neo hover:bg-orange-600',
    'pink': 'bg-[var(--color-accent-pink)] text-white shadow-neo hover:bg-pink-600',
    'red': 'bg-[var(--color-accent-red)] text-white shadow-neo hover:bg-red-600',
    'white': 'bg-white text-black shadow-neo hover:bg-gray-100'
  };
  
  return variants[props.variant] || variants.primary;
});

const sizeClasses = computed(() => {
  const sizes = {
    'sm': 'text-sm',
    'md': 'text-base',
    'lg': 'text-lg'
  };
  
  return sizes[props.size] || sizes.md;
});
</script>

<style>
.border-3 {
  border-width: 3px;
}

.shadow-neo {
  box-shadow: var(--shadow-neo);
}
</style> 