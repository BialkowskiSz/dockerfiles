#   Run alpine with shellcheck and find/file/grep
#
# Usage: (where test.sh is test script)
#   docker run --rm -it \
#       --name my_shellcheck \
#       -v $(pwd):/usr/src:ro \
#       --workdir /usr/src \
#       bialkowskisz/shellcheck ./test.sh

FROM koalaman/shellcheck-alpine

LABEL maintainer "Szymon Bialkowski <bialkowski.sz@gmail.com>"

RUN apk update && apk add bash grep file

CMD ["shellcheck"]
