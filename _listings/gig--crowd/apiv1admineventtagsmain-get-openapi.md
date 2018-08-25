---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Admin Event Tags Main
  version: 1.0.0
  description: Get admin event tags main.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/event/{page}:
    get:
      summary: Get Admin Event Page
      description: Get admin event page.
      operationId: getApiV1AdminEventPage
      x-api-path-slug: apiv1admineventpage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.cityId
      - in: query
        name: request.from
      - in: query
        name: request.isRecommended
      - in: query
        name: request.placeId
      - in: query
        name: request.placeName
      - in: query
        name: request.query
      - in: query
        name: request.status
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Page
  /api/v1/admin/event/approve/{eventId}:
    post:
      summary: Post Admin Event Approve Eventid
      description: Post admin event approve eventid.
      operationId: postApiV1AdminEventApproveEvent
      x-api-path-slug: apiv1admineventapproveeventid-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Approve
      - Eventid
  /api/v1/admin/event/reject:
    post:
      summary: Post Admin Event Reject
      description: Post admin event reject.
      operationId: postApiV1AdminEventReject
      x-api-path-slug: apiv1admineventreject-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Reject
  /api/v1/admin/event/defer:
    post:
      summary: Post Admin Event Defer
      description: Post admin event defer.
      operationId: postApiV1AdminEventDefer
      x-api-path-slug: apiv1admineventdefer-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Defer
  /api/v1/admin/event/add:
    post:
      summary: Post Admin Event Add
      description: Post admin event add.
      operationId: postApiV1AdminEventAdd
      x-api-path-slug: apiv1admineventadd-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: event
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
  /api/v1/admin/event/tags/main:
    get:
      summary: Get Admin Event Tags Main
      description: Get admin event tags main.
      operationId: getApiV1AdminEventTagsMain
      x-api-path-slug: apiv1admineventtagsmain-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Tags
      - Main
  /api/v1/admin/event/tags/additional:
    get:
      summary: Get Admin Event Tags Additional
      description: Get admin event tags additional.
      operationId: getApiV1AdminEventTagsAdditional
      x-api-path-slug: apiv1admineventtagsadditional-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Tags
      - Itional
  /api/v1/admin/event/{eventId}/thumbnail/url:
    post:
      summary: Post Admin Event Eventid Thumbnail Url
      description: Post admin event eventid thumbnail url.
      operationId: postApiV1AdminEventEventThumbnailUrl
      x-api-path-slug: apiv1admineventeventidthumbnailurl-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: body
        name: url
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Eventid
      - Thumbnail
      - Url
  /api/v1/admin/event/{primaryId}/merge/{secondaryId}:
    get:
      summary: Get Admin Event Primaryid Merge Secondaryid
      description: Get admin event primaryid merge secondaryid.
      operationId: getApiV1AdminEventPrimaryMergeSecondary
      x-api-path-slug: apiv1admineventprimaryidmergesecondaryid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: primaryId
      - in: path
        name: secondaryId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Primaryid
      - Merge
      - Secondaryid
  /api/v1/admin/event/statistic:
    get:
      summary: Get Admin Event Statistic
      description: Get admin event statistic.
      operationId: getApiV1AdminEventStatistic
      x-api-path-slug: apiv1admineventstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Statistic
  /api/v1/admin/moderator/statistic:
    get:
      summary: Get Admin Moderator Statistic
      description: Get admin moderator statistic.
      operationId: getApiV1AdminModeratorStatistic
      x-api-path-slug: apiv1adminmoderatorstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Moderator
      - Statistic
  /api/v1/admin/parser/config:
    get:
      summary: Get Admin Parser Config
      description: Get admin parser config.
      operationId: getApiV1AdminParserConfig
      x-api-path-slug: apiv1adminparserconfig-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Config
  /api/v1/admin/parser/all:
    get:
      summary: Get Admin Parser All
      description: Get admin parser all.
      operationId: getApiV1AdminParserAll
      x-api-path-slug: apiv1adminparserall-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
  /api/v1/admin/parser/logs:
    get:
      summary: Get Admin Parser Logs
      description: Get admin parser logs.
      operationId: getApiV1AdminParserLogs
      x-api-path-slug: apiv1adminparserlogs-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: request.from
      - in: query
        name: request.query
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Logs
  /api/v1/admin/parser/statistic:
    get:
      summary: Get Admin Parser Statistic
      description: Get admin parser statistic.
      operationId: getApiV1AdminParserStatistic
      x-api-path-slug: apiv1adminparserstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Statistic
  /api/v1/admin/parser/log/error:
    post:
      summary: Post Admin Parser Log Error
      description: Post admin parser log error.
      operationId: postApiV1AdminParserLogError
      x-api-path-slug: apiv1adminparserlogerror-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Log
      - Error
  /api/v1/admin/place/{page}:
    get:
      summary: Get Admin Place Page
      description: Get admin place page.
      operationId: getApiV1AdminPlacePage
      x-api-path-slug: apiv1adminplacepage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.cityId
      - in: query
        name: request.isRecommended
      - in: query
        name: request.query
      - in: query
        name: request.status
      - in: query
        name: request.url
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Page
  /api/v1/admin/place/{placeId}:
    put:
      summary: Put Admin Place Placeid
      description: Put admin place placeid.
      operationId: putApiV1AdminPlacePlace
      x-api-path-slug: apiv1adminplaceplaceid-put
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: placeId
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
    delete:
      summary: Delete Admin Place Placeid
      description: Delete admin place placeid.
      operationId: deleteApiV1AdminPlacePlace
      x-api-path-slug: apiv1adminplaceplaceid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
  /api/v1/admin/place:
    post:
      summary: Post Admin Place
      description: Post admin place.
      operationId: postApiV1AdminPlace
      x-api-path-slug: apiv1adminplace-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
  /api/v1/admin/place/{placeId}/thumbnail:
    post:
      summary: Post Admin Place Placeid Thumbnail
      description: Post admin place placeid thumbnail.
      operationId: postApiV1AdminPlacePlaceThumbnail
      x-api-path-slug: apiv1adminplaceplaceidthumbnail-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
      - Thumbnail
  /api/v1/admin/place/{placeId}/photos:
    post:
      summary: Post Admin Place Placeid Photos
      description: Post admin place placeid photos.
      operationId: postApiV1AdminPlacePlacePhotos
      x-api-path-slug: apiv1adminplaceplaceidphotos-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
      - Photos
  /api/v1/admin/place/{placeId}/photo/{photoId}:
    delete:
      summary: Delete Admin Place Placeid Photo Photoid
      description: Delete admin place placeid photo photoid.
      operationId: deleteApiV1AdminPlacePlacePhotoPhoto
      x-api-path-slug: apiv1adminplaceplaceidphotophotoid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: photoId
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
      - Photo
      - Photoid
  /api/v1/admin/place/{placeId}/confirm:
    put:
      summary: Put Admin Place Placeid Confirm
      description: Put admin place placeid confirm.
      operationId: putApiV1AdminPlacePlaceConfirm
      x-api-path-slug: apiv1adminplaceplaceidconfirm-put
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
      - Confirm
  /api/v1/admin/place/tags/main:
    get:
      summary: Get Admin Place Tags Main
      description: Get admin place tags main.
      operationId: getApiV1AdminPlaceTagsMain
      x-api-path-slug: apiv1adminplacetagsmain-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Tags
      - Main
  /api/v1/admin/place/tags/additional:
    get:
      summary: Get Admin Place Tags Additional
      description: Get admin place tags additional.
      operationId: getApiV1AdminPlaceTagsAdditional
      x-api-path-slug: apiv1adminplacetagsadditional-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Tags
      - Itional
  /api/v1/admin/place/{primaryId}/merge/{secondaryId}:
    get:
      summary: Get Admin Place Primaryid Merge Secondaryid
      description: Get admin place primaryid merge secondaryid.
      operationId: getApiV1AdminPlacePrimaryMergeSecondary
      x-api-path-slug: apiv1adminplaceprimaryidmergesecondaryid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: primaryId
      - in: path
        name: secondaryId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Primaryid
      - Merge
      - Secondaryid
  /api/v1/admin/place/statistic:
    get:
      summary: Get Admin Place Statistic
      description: Get admin place statistic.
      operationId: getApiV1AdminPlaceStatistic
      x-api-path-slug: apiv1adminplacestatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Statistic
  /api/v1/admin/placeReview/{page}:
    get:
      summary: Get Admin Placereview Page
      description: Get admin placereview page.
      operationId: getApiV1AdminPlacereviewPage
      x-api-path-slug: apiv1adminplacereviewpage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.placeName
      - in: query
        name: request.status
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Placereview
      - Page
  /api/v1/admin/placeReview/{reviewId}/confirm:
    post:
      summary: Post Admin Placereview Reviewid Confirm
      description: Post admin placereview reviewid confirm.
      operationId: postApiV1AdminPlacereviewReviewConfirm
      x-api-path-slug: apiv1adminplacereviewreviewidconfirm-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Placereview
      - Reviewid
      - Confirm
  /api/v1/admin/placeReview/{reviewId}/reject:
    post:
      summary: Post Admin Placereview Reviewid Reject
      description: Post admin placereview reviewid reject.
      operationId: postApiV1AdminPlacereviewReviewReject
      x-api-path-slug: apiv1adminplacereviewreviewidreject-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: reason
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Placereview
      - Reviewid
      - Reject
  /api/v1/admin/promocode/generate:
    get:
      summary: Get Admin Promocode Generate
      description: Get admin promocode generate.
      operationId: getApiV1AdminPromocodeGenerate
      x-api-path-slug: apiv1adminpromocodegenerate-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Generate
  /api/v1/admin/promocode/{page}:
    get:
      summary: Get Admin Promocode Page
      description: Get admin promocode page.
      operationId: getApiV1AdminPromocodePage
      x-api-path-slug: apiv1adminpromocodepage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.used
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Page
  /api/v1/admin/promocode:
    post:
      summary: Post Admin Promocode
      description: Post admin promocode.
      operationId: postApiV1AdminPromocode
      x-api-path-slug: apiv1adminpromocode-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
  /api/v1/admin/promocode/{promoCodeId}:
    put:
      summary: Put Admin Promocode Promocodeid
      description: Put admin promocode promocodeid.
      operationId: putApiV1AdminPromocodePromocode
      x-api-path-slug: apiv1adminpromocodepromocodeid-put
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: promoCodeId
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Promocodeid
    delete:
      summary: Delete Admin Promocode Promocodeid
      description: Delete admin promocode promocodeid.
      operationId: deleteApiV1AdminPromocodePromocode
      x-api-path-slug: apiv1adminpromocodepromocodeid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: promoCodeId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Promocodeid
  /api/v1/admin/settings/{userId}:
    get:
      summary: Get Admin Settings Userid
      description: Get admin settings userid.
      operationId: getApiV1AdminSettingsUser
      x-api-path-slug: apiv1adminsettingsuserid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Settings
      - Userid
    post:
      summary: Post Admin Settings Userid
      description: Post admin settings userid.
      operationId: postApiV1AdminSettingsUser
      x-api-path-slug: apiv1adminsettingsuserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Settings
      - Userid
  /api/v1/admin/statistics:
    get:
      summary: Get Admin Statistics
      description: Get admin statistics.
      operationId: getApiV1AdminStatistics
      x-api-path-slug: apiv1adminstatistics-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Statistics
  /api/v1/admin/statistics/{type}:
    get:
      summary: Get Admin Statistics Type
      description: Get admin statistics type.
      operationId: getApiV1AdminStatisticsType
      x-api-path-slug: apiv1adminstatisticstype-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Statistics
      - Type
  /api/v1/admin/transactions:
    get:
      summary: Get Admin Transactions
      description: Get admin transactions.
      operationId: getApiV1AdminTransactions
      x-api-path-slug: apiv1admintransactions-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Transactions
  /api/v1/admin/transactions/{filter}:
    get:
      summary: Get Admin Transactions Filter
      description: Get admin transactions filter.
      operationId: getApiV1AdminTransactionsFilter
      x-api-path-slug: apiv1admintransactionsfilter-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: filter
      - in: query
        name: range.from
      - in: query
        name: range.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Transactions
      - Filter
  /api/v1/admin/user:
    get:
      summary: Get Admin User
      description: Get admin user.
      operationId: getApiV1AdminUser
      x-api-path-slug: apiv1adminuser-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: filter.email
      - in: query
        name: filter.emailConfirmed
      - in: query
        name: filter.phoneConfirmed
      - in: query
        name: filter.phoneNumber
      - in: query
        name: filter.roleId
      - in: query
        name: filter.status
      - in: query
        name: filter.userName
      - in: query
        name: page
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
  /api/v1/admin/user/{userId}/avatar:
    post:
      summary: Post Admin User Userid Avatar
      description: Post admin user userid avatar.
      operationId: postApiV1AdminUserUserAvatar
      x-api-path-slug: apiv1adminuseruseridavatar-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Userid
      - Avatar
  /api/v1/admin/user/roles/{userId}:
    get:
      summary: Get Admin User Roles Userid
      description: Get admin user roles userid.
      operationId: getApiV1AdminUserRolesUser
      x-api-path-slug: apiv1adminuserrolesuserid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Roles
      - Userid
    post:
      summary: Post Admin User Roles Userid
      description: Post admin user roles userid.
      operationId: postApiV1AdminUserRolesUser
      x-api-path-slug: apiv1adminuserrolesuserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: roles
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Roles
      - Userid
  /api/v1/admin/user/roles:
    get:
      summary: Get Admin User Roles
      description: Get admin user roles.
      operationId: getApiV1AdminUserRoles
      x-api-path-slug: apiv1adminuserroles-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Roles
  /api/v1/admin/user/empty/{role}:
    get:
      summary: Get Admin User Empty Role
      description: Get admin user empty role.
      operationId: getApiV1AdminUserEmptyRole
      x-api-path-slug: apiv1adminuseremptyrole-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: role
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Empty
      - Role
  /api/v1/admin/user/client/{userId}:
    get:
      summary: Get Admin User Client Userid
      description: Get admin user client userid.
      operationId: getApiV1AdminUserClientUser
      x-api-path-slug: apiv1adminuserclientuserid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Client
      - Userid
    post:
      summary: Post Admin User Client Userid
      description: Post admin user client userid.
      operationId: postApiV1AdminUserClientUser
      x-api-path-slug: apiv1adminuserclientuserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Client
      - Userid
  /api/v1/admin/user/emailAndPhone/{userId}:
    post:
      summary: Post Admin User Emailandphone Userid
      description: Post admin user emailandphone userid.
      operationId: postApiV1AdminUserEmailandphoneUser
      x-api-path-slug: apiv1adminuseremailandphoneuserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - User
      - Emailandphone
      - Userid
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---