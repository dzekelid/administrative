---
swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 1
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeProductAsAdmin:
    get:
      summary: Describe Product As Admin
      description: |-
        Retrieves information about a specified product, run with administrator
                 access.
      operationId: describeProductAsAdmin
      x-api-path-slug: actiondescribeproductasadmin-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the product for which to retrieve information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=SearchProductsAsAdmin:
    get:
      summary: Search Products As Admin
      description: |-
        Retrieves summary and status information about all products created within the
                 caller's account.
      operationId: searchProductsAsAdmin
      x-api-path-slug: actionsearchproductsasadmin-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Filters
        description: The list of filters with which to limit search results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductSource
        description: Access level of the source of the product
        type: string
      - in: query
        name: SortBy
        description: The sort field specifier
        type: string
      - in: query
        name: SortOrder
        description: The sort order specifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
---