apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
  name: {{ values.component_id | dump }}
  description: An AI-powered project secured by the Project Shield.
  annotations:
    # 🔗 Link this to the Dev Spaces dashboard automatically
    che.eclipse.org/devworkspace-id: {{ values.component_id }}
spec:
  type: service
  lifecycle: experimental
  owner: {{ values.owner | dump }}