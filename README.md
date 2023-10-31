 
 possible components for our project 
1. **Authentication**:
   - `Authentication`: Handles user registration and authentication.
     - Routes: `/register`, `/login`

2. **Navigation**:
   - `NavigationBar`: Reusable navigation bar or header component with links to different sections of the application, user profile, settings, etc.
   - `SidebarMenu`: Sidebar menu for quick access to major sections of the application, including links to user requests, asset management, reports, etc.

3. **Notifications and Feedback**:
   - `ErrorMessages`: Component to display error messages to users for validation errors or server-side issues.
   - `ConfirmationModals`: Modal components for confirming critical actions like deleting an asset or approving a request.
   - `ToastNotifications`: Toast notifications for non-intrusive feedback about successful actions.

4. **Data Management** (Restricted to Admin and Procurement Manager):
   - `DataManagement`: Manages asset data, including adding, updating, and removing data.
     - Routes: `/add_data`, `/update_data/<int:data_id>`, `/remove_data/<int:data_id>`

5. **Request Management** (Restricted to Procurement Manager):
   - `RequestManagement`: Handles approval of asset requests and provides routes for viewing pending and completed requests.
     - Routes: `/approve_request/<int:request_id>`, `/manager_pending_requests`, `/manager_completed_requests`

6. **User Requests**:
   - `UserRequests`: Allows users to view their active and completed requests.
     - Routes: `/user_requests`

7. **Search and Filtering**:
   - `SearchBar`: Component for users to search for specific assets, requests, or other data within the application.
   - `Filtering`: Allows users to filter data based on various criteria.

8. **User Profile**:
   - `UserProfile`: Component for users to view and edit their profile information.
     - Routes: `/profile`

9. **Form Handling**:
   - `FormComponents`: Reusable form components for various data entry tasks, including forms for adding new assets, updating profiles, or submitting asset requests. These components handle form validation and submission.


11. **Asset Management**:
   - `AssetManagement`: Manages assets including adding new assets.
     - Routes: `/add_asset`
     
   - `AssetAllocation`: Manages asset allocation to employees.
     - Routes: `/allocate_asset/<int:asset_id>`

   - `AssetRequest`: Manages asset requests submitted by employees.
     - Routes: `/request_asset/<int:asset_id>`

12. **User Classification**:
    - `UserClassification`: Classifies users based on their roles.
      - Routes: `/classify`

13. **Manager Operations**:
    - `ManagerOperations`: Handles manager-specific operations such as approving requests and managing assets.
      - Routes: `/approve_request/<int:request_id>`, `/manager_pending_requests`, `/manager_completed_requests`, `/add_asset`, `/allocate_asset/<int:asset_id>`

14. **User Requests Viewing**:
    - `UserRequestsView`: Allows users to view their active and completed requests.
      - Routes: `/user_requests`

