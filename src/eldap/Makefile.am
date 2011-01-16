## Licensed under the Apache License, Version 2.0 (the "License"); you may not
## use this file except in compliance with the License. You may obtain a copy of
## the License at
##
##   http://www.apache.org/licenses/LICENSE-2.0
##
## Unless required by applicable law or agreed to in writing, software
## distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
## WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
## License for the specific language governing permissions and limitations under
## the License.

eldapebindir = $(localerlanglibdir)/eldap/ebin

eldap_file_collection = \
    eldap.erl \
    ELDAPv3.erl

eldapebin_make_generated_file_list = \
    eldap.beam \
    ELDAPv3.beam

eldapebin_DATA = \
    $(eldapebin_make_generated_file_list)

EXTRA_DIST =  \
    $(eldap_file_collection) \
	eldap.hrl \
    ELDAPv3.hrl

CLEANFILES = \
    $(eldapebin_make_generated_file_list)

%.beam: %.erl
	$(ERLC) $(ERLC_FLAGS) $<
