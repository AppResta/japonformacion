---
title: "Checkout"
permalink: /checkout/
---

# Checkout

<script>
document.addEventListener('DOMContentLoaded', function() {
  console.log('Checkout page loaded');

  const urlParams = new URLSearchParams(window.location.search);
  const plan = urlParams.get('plan');
  console.log('Plan selected:', plan);

  // Display the selected plan dynamically
  const planElement = document.createElement('h2');
  planElement.textContent = plan ? 'Plan Seleccionado: ' + plan : 'No se ha seleccionado ningún plan';
  
  // Insert the plan element below the existing content
  const checkoutContent = document.querySelector('.page-content');
  checkoutContent.appendChild(planElement);
});
</script>
