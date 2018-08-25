---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Admin Set User Settings
  version: 1.0.0
  description: Sets all the user settings for a specified user name.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminAddUserToGroup:
    get:
      summary: Admin Add User To Group
      description: Adds the specified user to the specified group.
      operationId: adminAddUserToGroup
      x-api-path-slug: actionadminaddusertogroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminConfirmSignUp:
    get:
      summary: Admin Confirm Sign Up
      description: Confirms user registration as an admin without using a confirmation
        code.
      operationId: adminConfirmSignUp
      x-api-path-slug: actionadminconfirmsignup-get
      parameters:
      - in: query
        name: Username
        description: The user name for which you want to confirm user registration
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for which you want to confirm user registration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sign Up
  /?Action=AdminCreateUser:
    get:
      summary: Admin Create User
      description: |-
        Creates a new user in the specified user pool and sends a welcome message via email
                    or phone (SMS).
      operationId: adminCreateUser
      x-api-path-slug: actionadmincreateuser-get
      parameters:
      - in: query
        name: DesiredDeliveryMediums
        description: Specify EMAIL if email will be used to send the welcome message
        type: string
      - in: query
        name: ForceAliasCreation
        description: This parameter is only used if the phone_number_verified or email_verified            attribute
          is set to True
        type: string
      - in: query
        name: MessageAction
        description: Set to RESEND to resend the invitation message to a user that
          already exists and            reset the expiration limit on the users account
        type: string
      - in: query
        name: TemporaryPassword
        description: The users temporary password
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs that contain user attributes and
          attribute values to            be set for the user to be created
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where the user will be created
        type: string
      - in: query
        name: ValidationData
        description: The users validation data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDeleteUser:
    get:
      summary: Admin Delete User
      description: Deletes a user as an administrator.
      operationId: adminDeleteUser
      x-api-path-slug: actionadmindeleteuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to delete
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete the
          user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDeleteUserAttributes:
    get:
      summary: Admin Delete User Attributes
      description: Deletes the user attributes in a user pool as an administrator.
      operationId: adminDeleteUserAttributes
      x-api-path-slug: actionadmindeleteuserattributes-get
      parameters:
      - in: query
        name: UserAttributeNames
        description: An array of strings representing the user attribute names you
          wish to            delete
        type: string
      - in: query
        name: Username
        description: The user name of the user from which you would like to delete
          attributes
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete user            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDisableUser:
    get:
      summary: Admin Disable User
      description: Disables the specified user as an administrator.
      operationId: adminDisableUser
      x-api-path-slug: actionadmindisableuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to disable
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to disable
          the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminEnableUser:
    get:
      summary: Admin Enable User
      description: Enables the specified user as an administrator.
      operationId: adminEnableUser
      x-api-path-slug: actionadminenableuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to enable
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to enable the
          user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminForgetDevice:
    get:
      summary: Admin Forget Device
      description: Forgets the device, as an administrator.
      operationId: adminForgetDevice
      x-api-path-slug: actionadminforgetdevice-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=AdminGetDevice:
    get:
      summary: Admin Get Device
      description: Gets the device, as an administrator.
      operationId: adminGetDevice
      x-api-path-slug: actionadmingetdevice-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php
  /?Action=AdminGetUser:
    get:
      summary: Admin Get User
      description: Gets the specified user by user name in a user pool as an administrator.
      operationId: adminGetUser
      x-api-path-slug: actionadmingetuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to retrieve
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to get information
          about the            user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminInitiateAuth:
    get:
      summary: Admin Initiate Auth
      description: Initiates the authentication flow, as an administrator.
      operationId: adminInitiateAuth
      x-api-path-slug: actionadmininitiateauth-get
      parameters:
      - in: query
        name: AuthFlow
        description: The authentication flow
        type: string
      - in: query
        name: AuthParameters
        description: The authentication parameters
        type: string
      - in: query
        name: ClientId
        description: The client app ID
        type: string
      - in: query
        name: ClientMetadata
        description: The client app metadata
        type: string
      - in: query
        name: UserPoolId
        description: The ID of the Amazon Cognito user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authnetication
  /?Action=AdminListDevices:
    get:
      summary: Admin List Devices
      description: Lists devices, as an administrator.
      operationId: adminListDevices
      x-api-path-slug: actionadminlistdevices-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the devices request
        type: string
      - in: query
        name: PaginationToken
        description: The pagination token
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php
  /?Action=AdminListGroupsForUser:
    get:
      summary: Admin List Groups For User
      description: Lists the groups that the user belongs to.
      operationId: adminListGroupsForUser
      x-api-path-slug: actionadminlistgroupsforuser-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the request to list groups
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminRemoveUserFromGroup:
    get:
      summary: Admin Remove User From Group
      description: Removes the specified user from the specified group.
      operationId: adminRemoveUserFromGroup
      x-api-path-slug: actionadminremoveuserfromgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminResetUserPassword:
    get:
      summary: Admin Reset User Password
      description: Resets the specified user's password in a user pool as an administrator.
      operationId: adminResetUserPassword
      x-api-path-slug: actionadminresetuserpassword-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user whose password you wish to reset
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to reset the
          users            password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Passwords
  /?Action=AdminRespondToAuthChallenge:
    get:
      summary: Admin Respond To Auth Challenge
      description: Responds to an authentication challenge, as an administrator.
      operationId: adminRespondToAuthChallenge
      x-api-path-slug: actionadminrespondtoauthchallenge-get
      parameters:
      - in: query
        name: ChallengeName
        description: The name of the challenge
        type: string
      - in: query
        name: ChallengeResponses
        description: The challenge response
        type: string
      - in: query
        name: ClientId
        description: The client ID
        type: string
      - in: query
        name: Session
        description: The session
        type: string
      - in: query
        name: UserPoolId
        description: The ID of the Amazon Cognito user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authentication Challenge
  /?Action=AdminSetUserSettings:
    get:
      summary: Admin Set User Settings
      description: Sets all the user settings for a specified user name.
      operationId: adminSetUserSettings
      x-api-path-slug: actionadminsetusersettings-get
      parameters:
      - in: query
        name: MFAOptions
        description: Specifies the options for MFA (e
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you wish to set user settings
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to set the
          users settings, such            as MFA options
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
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