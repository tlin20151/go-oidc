# go-oidc

[![GoDoc](https://godoc.org/github.com/tlin20151/go-oidc?status.svg)](https://godoc.org/github.com/coreos/go-oidc)
[![Build Status](https://travis-ci.org/tlin20151/go-oidc.png?branch=keycloak-gatekeeper_patch)](https://travis-ci.org/tlin20151/go-oidc)

This repo is taken directly from coreos/go-oidc (https://github.com/coreos/go-oidc) and being customized to resolve the following issues:
1. comment out the logic to return errors immediately when issuers were mismatched
2. comment out the logic to always include openid+email+profile in its scope.  Changed it so the default scope will only require openid. 
