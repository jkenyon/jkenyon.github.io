<div class="alert alert-{{ include.color | default: 'warning' }} {% if include.align %}text-{{ include.align }}{% endif %}" role="alert" markdown="1">
{{ include.text }}
</div>