
NODEUNIT=../node_modules/nodeunit/bin/nodeunit

.PHONY: test
test:
	NODE_PATH=node_modules $(NODEUNIT) test.js

# Test will all node versions (presumes install locations I use on my machine).
.PHONY: testall
testall: test08 test10 test06 test04


.PHONY: test08
test08:
	@echo "# Test node 0.8.x (with node `$(HOME)/opt/node-0.8/bin/node --version`)"
	PATH="$(HOME)/opt/node-0.8/bin:$(PATH)" $(NODEUNIT) test.js
.PHONY: test10
test10:
	@echo "# Test node 0.10.x (with node `$(HOME)/opt/node-0.10/bin/node --version`)"
	PATH="$(HOME)/opt/node-0.10/bin:$(PATH)" $(NODEUNIT) test.js
.PHONY: test06
test06:
	@echo "# Test node 0.6.x (with node `$(HOME)/opt/node-0.6/bin/node --version`)"
	PATH="$(HOME)/opt/node-0.6/bin:$(PATH)" $(NODEUNIT) test.js
.PHONY: test04
test04:
	@echo "# Test node 0.4.x (with node `$(HOME)/opt/node-0.4/bin/node --version`)"
	PATH="$(HOME)/opt/node-0.4/bin:$(PATH)" $(NODEUNIT) test.js
