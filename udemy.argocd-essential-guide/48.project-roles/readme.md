$ unset ARGOCD_AUTH_TOKEN

$ argocd logout 192.168.35.80:32114

$ argocd login 192.168.35.80:32114 --username admin --password test1234 --insecure --grpc-web

$ argocd proj role create-token project-with-role ci-role
Create token succeeded for proj:project-with-role:ci-role.
  ID: 9027b42e-405a-4750-9e45-1fb6242b05aa
  Issued At: 2026-01-07T23:24:59+09:00
  Expires At: Never
  Token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJhcmdvY2QiLCJzdWIiOiJwcm9qOnByb2plY3Qtd2l0aC1yb2xlOmNpLXJvbGUiLCJuYmYiOjE3Njc3OTU4OTksImlhdCI6MTc2Nzc5NTg5OSwianRpIjoiOTAyN2I0MmUtNDA1YS00NzUwLTllNDUtMWZiNjI0MmIwNWFhIn0.GEXxWVA_A3GE9XnegpM_on7txLNuqMPoCfWWh3ZfRwo

  $ argocd app list

  $ argocd app delete guestbook-dev-project --auth-token eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJhcmdvY2QiLCJzdWIiOiJwcm9qOnByb2plY3Qtd2l0aC1yb2xlOmNpLXJvbGUiLCJuYmYiOjE3Njc3OTU4OTksImlhdCI6MTc2Nzc5NTg5OSwianRpIjoiOTAyN2I0MmUtNDA1YS00NzUwLTllNDUtMWZiNjI0MmIwNWFhIn0.GEXxWVA_A3GE9XnegpM_on7txLNuqMPoCfWWh3ZfRwo