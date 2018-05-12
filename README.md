# apollo-client-issue-2533

Demonstrates that the problem outlined in 
https://github.com/apollographql/apollo-client/issues/2533 is no longer an 
issue (using current Apollo libraries).

```
git clone https://github.com/hwillson/apollo-client-issue-2533.git
cd apollo-client-issue-2533
npm install
npm start
```

Go to http://localhost:3000/ then:

1. Press Fetch more.
2. Block incoming connections from http://localhost:3001/graphql (e.g. 
   use Chrome's Network Offline mode).
3. Press Fetch more one more time, which errors (expected behaviour).
4. Unblock incoming connections.
5. Finally, press Fetch more and new content will be added.
