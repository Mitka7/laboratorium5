# laboratorium5
# Proces budowania obrazu Docker z wykorzystaniem argumentu VERSION.
```
docker build --build-arg VERSION=v1.0.0 -t lab5:v1 .
```
<img width="916" height="717" alt="image" src="https://github.com/user-attachments/assets/914f5c58-c0be-4d46-bd25-d8b0449634fb" />

# Uruchomienie kontenerów na podstawie zbudowanego wcześniej obrazu.
```
docker run -d -p 8080:80 --name nlab5 --hostname lab5 lab5:v1
```
<img width="921" height="73" alt="image" src="https://github.com/user-attachments/assets/c9c0404b-43d7-4937-88e1-06ee1d4b386a" />

```
docker run -d -p 8081:80 --name nlab5_2 --hostname lab5_2 lab5:v1
```
<img width="927" height="69" alt="image" src="https://github.com/user-attachments/assets/4d979bc4-83f3-4889-9de9-1ac455b82fc8" />

# Weryfikacja stanu uruchomionych kontenerów oraz działanie mechanizmu HEALTHCHECK.

```
docker ps
```
<img width="923" height="182" alt="image" src="https://github.com/user-attachments/assets/b3d34a38-c2ba-40de-b304-906f10e240f4" />

# Widok strony głównej aplikacji dla pierwszej instancji kontenera.

<img width="481" height="376" alt="image" src="https://github.com/user-attachments/assets/7fa527d4-f947-4af9-b0a1-c3172c2bdc30" />

# Widok strony głównej aplikacji dla drugiej instancji kontenera.

<img width="734" height="414" alt="image" src="https://github.com/user-attachments/assets/c50ca845-14df-4fcd-b15b-643788ff8042" />

