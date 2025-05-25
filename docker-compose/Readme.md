docker-compose up --build


<!-- aamirbelalkhan@Aamirs-MacBook-Air ~/Desktop/Docker/docker-compose %docker-compose up --build
WARN[0000] /Users/aamirbelalkhan/Desktop/Docker/docker-compose/docker-compose.yml: the attribute `version` is obsolete, it will be ignored, please remove it to avoid potential confusion 
Compose now can delegate build to bake for better performances
Just set COMPOSE_BAKE=true
[+] Building 0.0s (0/0)  docker:deskt[+] Building 0.0s (0/1)  docker:deskt[+] Building 0.2s (1/2)  docker:deskt[+] Building 0.3s (1/2)  docker:deskt[+] Building 0.5s (1/2)  docker:deskt[+] Building 0.6s (1/2)  docker:deskt[+] Building 0.8s (1/2)  docker:deskt[+] Building 0.9s (1/2)  docker:deskt[+] Building 1.0s (2/2)  docker:deskt[+] Building 1.1s (7/12)  docker:desk[+] Building 1.3s (7/12)  docker:desk[+] Building 1.4s (7/12)  docker:desk[+] Building 1.6s (7/12)  docker:desk[+] Building 1.7s (7/12)  docker:desk[+] Building 1.9s (7/12)  docker:desk[+] Building 2.0s (7/12)  docker:desk[+] Building 2.2s (7/12)  docker:desk[+] Building 2.3s (7/12)  docker:desk[+] Building 2.5s (7/12)  docker:des[+] Building 9.1s (25/25) FINISHED                       docker:desktop-linux
 => [backend internal] load build definition from Dockerfile             0.0s
 => => transferring dockerfile: 656B                                     0.0s
 => [frontend internal] load metadata for docker.io/library/node:18-alp  1.5s
 => [backend internal] load .dockerignore                                0.0s
 => => transferring context: 165B                                        0.0s
 => [frontend 1/8] FROM docker.io/library/node:18-alpine@sha256:8d6421d  0.0s
 => [backend internal] load build context                                0.0s
 => => transferring context: 55.77kB                                     0.0s
 => CACHED [frontend 2/8] WORKDIR /app                                   0.0s
 => [backend 3/8] COPY package*.json ./                                  0.0s
 => [backend 4/8] RUN npm ci                                             3.0s
 => [backend 5/8] COPY . .                                               0.1s
 => [backend 6/8] RUN addgroup -g 1001 -S nodejs                         0.3s
 => [backend 7/8] RUN adduser -S nextjs -u 1001                          0.3s
 => [backend 8/8] RUN chown -R nextjs:nodejs /app                        2.6s
 => [backend] exporting to image                                         0.5s
 => => exporting layers                                                  0.5s
 => => writing image sha256:c1d28552b0c6ca171cc9bea60a0115b38dbce29831a  0.0s
 => => naming to docker.io/library/docker-compose-backend                0.0s
 => [backend] resolving provenance for metadata file                     0.0s
 => [frontend internal] load build definition from Dockerfile            0.0s
 => => transferring dockerfile: 667B                                     0.0s
 => [frontend internal] load .dockerignore                               0.0s
 => => transferring context: 176B                                        0.0s
 => [frontend internal] load build context                               0.0s
 => => transferring context: 2.00kB                                      0.0s
 => CACHED [frontend 3/8] COPY package*.json ./                          0.0s
 => CACHED [frontend 4/8] RUN npm ci                                     0.0s
 => CACHED [frontend 5/8] COPY . .                                       0.0s
 => CACHED [frontend 6/8] RUN addgroup -g 1001 -S nodejs                 0.0s
 => CACHED [frontend 7/8] RUN adduser -S nextjs -u 1001                  0.0s
 => CACHED [frontend 8/8] RUN chown -R nextjs:nodejs /app                0.0s
 => [frontend] exporting to image                                        0.0s
 => => exporting layers                                                  0.0s
 => => writing image sha256:079d1b885fdbbc34a345caa24fedb93c0787d52f3ab  0.0s
 => => naming to docker.io/library/docker-compose-frontend               0.0s
 => [frontend] resolving provenance for metadata file                    0.1s
[+] Running 4/4
 ✔ backend                  Built                                        0.0s 
 ✔ frontend                 Built                                        0.0s 
 ✔ Container mern_frontend  Created                                      0.6s 
 ✔ Container mern_backend   Recreated                                    0.2s 
Attaching to mern_backend, mern_frontend
mern_frontend  | 
mern_frontend  | > frontend@0.0.0 dev
mern_frontend  | > vite --host 0.0.0.0
mern_frontend  | 
mern_backend   | 
mern_backend   | > backend@1.0.0 start
mern_backend   | > node server.js
mern_backend   | 
mern_frontend  | 
mern_frontend  |   VITE v6.3.5  ready in 392 ms
mern_frontend  | 
mern_frontend  |   ➜  Local:   http://localhost:5173/
mern_frontend  |   ➜  Network: http://172.22.0.3:5173/
mern_backend   | The server is running on the http://localhost:5002
mern_backend   | ✅ mongodb is connected


v View in Docker Desktop   o View Config   w Enable Watch -->