# FROM image:tag
    build the image start from the image we choose

# LABEL
    LABEL AUTHOR=nikko
    just only create meta information. not affected in the build or running container

# COPY source destination
    COPY src .
    COPY src ./src
    Copy file or folder from host(source) to container(destination)

# ENV
    ENV DB_USER=root
    add env in the build phase

# EXPOSE
    EXPOSE 8080
    expose the port, just for documentation

# RUN
    RUN npm install
    execute commands in the build phase, not at the running container

# CMD
    CMD ["npm", "start"]
    execute commands when container starts