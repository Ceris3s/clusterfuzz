# Copyright 2019 Google LLC
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
FROM gcr.io/clusterfuzz-images/base@sha256:1110514de5bb678562b75e5cf65130923bd22bb9371dcbc9e99483fd277ac135

RUN apt-get update && apt-get install -y openssh-client

ENV OS_OVERRIDE FUCHSIA
ENV QUEUE_OVERRIDE FUCHSIA
ENV FUCHSIA_USE_KVM 1

COPY start.sh /data/start.sh
