<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	testissuesamplesdk "github.com/speakeasy-sdks/test-issue-sample-sdk"
	"log"
)

func main() {
	s := testissuesamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->