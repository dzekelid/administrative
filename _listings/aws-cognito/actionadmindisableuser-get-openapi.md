---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Admin Disable User
  version: 1.0.0
  description: Disables the specified user as an administrator.
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