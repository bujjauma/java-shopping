---
apiVersion: v1
kind: Service
metadata:
 name: shopfront
 labels:
 app: shopfront
spec:
 type: NodePort
 selector:
 app: shopfront
 ports:
 — protocol: TCP
 port: 8010
 name: http
