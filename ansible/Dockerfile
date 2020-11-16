FROM centos:centos8

ENV ANSIBLE_HOST_KEY_CHECKING false
ENV ANSIBLE_GATHERING smart
ENV ANSIBLE_RETRY_FILES_ENABLED false

RUN yum check-update; \
  yum install -y gcc libffi-devel python3 epel-release; \
  yum install -y sshpass openssh-clients; \
  pip3 install --upgrade pip; \
  pip3 install ansible lxml

ENTRYPOINT ["ansible-playbook","playbook.yml"]
