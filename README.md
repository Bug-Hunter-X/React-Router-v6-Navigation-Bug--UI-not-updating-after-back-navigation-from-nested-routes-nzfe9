# React Router v6 Navigation Bug

This repository demonstrates a subtle bug in React Router v6 related to unexpected behavior when navigating back from nested routes.  After navigating to a nested route and then using the browser's back button (or programmatic navigation back to the parent route), the UI might not update correctly. The URL might change but the content remains the same. 

The issue stems from how the history and `useLocation` or `useParams` hooks interact.   The solution demonstrates how to address this issue by leveraging the `useNavigate` hook with appropriate cleanup logic. 