# AssignmentRentomojo @thedeveloperyug


## Screenshots:
<img src="/ss11.png"></img>
<img src="/ss12.png"></img>
<img src="/ss13.png"></img>


## Database: psql
<h1>Set-up Database</h1>
<mark>sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list' </br>
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -  </br>
sudo apt-get update  </br>
sudo apt-get -y install postgresql </br>
</mark>

--------------------

U - postgres
P - *******

commands
-------------
sudo -i -u postgres #login postgres default user
psql #enter database management sys

\q =exit

createdb comments    #create databse with name 'comments'

psql -d comments  #enter in databse

\conninfo #gives conn details

\password postgres  # change the password

## Schema: Prisma

npx prisma migrate dev #for latest changes in db
npx prisma db seed # filling dummy data

## Backend Technology: Node Js
## install 
dependencies - npm i fastify dotenv @fastify/cookie @fastify/cors @fastify/sensible </br>
-------------- npm i axios

## RUN Server 
npm run devStart

## RUN CLient
npm start

