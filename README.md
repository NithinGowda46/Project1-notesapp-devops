# Project2-notesapp-devops


#always add this in gitignore ---kubectl apply -f "this file seperatly"
kind: Secret
apiVersion: v1
metadata:
  name: secret
  namespace: project-2
data:
  MYSQL_PASSWORD: bml0aGlu  #base64 encoded value of nithin
  