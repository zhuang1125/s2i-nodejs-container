FROM registry.access.redhat.com/ubi8/nodejs-12

# Add application sources
ADD . .

# Install the dependencies
RUN npm install yarn -g
RUN yarn install --ignore-scripts
RUN npm install --ignore-scripts

# Run script uses standard ways to run the application
CMD npm run -d start
